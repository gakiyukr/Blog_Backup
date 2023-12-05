## 源码

[LloydAsp/nfd: No Fraud / Node Forward Bot (github.com)](https://github.com/LloydAsp/nfd)

## 特点

- 基于 Workers 搭建，只要你的配额够，CF 不拉闸，那么就不存在跑路的问题。
- 0 成本，连域名都不需要。
- 接入反欺诈系统，当聊天对象有诈骗历史时，自动发出提醒。
- 支持屏蔽用户，避免被骚扰。

## 搭建方法

首先去 [@BotFather](https://t.me/BotFather) 创建一个新机器人，获取一个 API KEY。

![](https://i2.wp.com/s3-jp-ap-3.040407.xyz/oss/photos/Telegram_wsn7VPwCgT.png)

然后使用 `/setjoingroups` 命令禁止机器人被添加到群组。

![](https://i2.wp.com/s3-jp-ap-3.040407.xyz/oss/photos/Telegram_EdjRLw2maS.png)

![](https://i2.wp.com/s3-jp-ap-3.040407.xyz/oss/photos/Telegram_Y9NlSByOUs.png)

找一个获取 [UUID](https://www.uuidgenerator.net/) 的网站，随机获取一个 UUID。

![](https://i2.wp.com/s3-jp-ap-3.040407.xyz/oss/photos/msedge_kOZmNVCeNb.png)

使用 [@userinfobot](https://t.me/userinfobot) 获取你的 TGID。

![](https://i2.wp.com/s3-jp-ap-3.040407.xyz/oss/photos/Telegram_Srd32WwvGs.png)

然后前往 CF 控制台，创建一个示例 Workers。

![](https://i2.wp.com/s3-jp-ap-3.040407.xyz/oss/photos/msedge_28Cxm9Q58Z.png)

![](https://i2.wp.com/s3-jp-ap-3.040407.xyz/oss/photos/msedge_qHaQsIMW8F.png)

然后添加环境变量。

- `ENV_BOT_TOKEN` 变量，值为 Bot 的 Token
- `ENV_BOT_SECRET` 变量，值为 UUID
- `ENV_ADMIN_UID `变量，值为 TGID

![](https://i2.wp.com/s3-jp-ap-3.040407.xyz/oss/photos/msedge_MxgLqP6iIC.png)

![](https://i2.wp.com/s3-jp-ap-3.040407.xyz/oss/photos/msedge_zMJMd316LF.png)

新建一个名字叫做 `nfd` 的 KV 数据库。

![](https://i2.wp.com/s3-jp-ap-3.040407.xyz/oss/photos/msedge_Dq8K6fgyuO.png)

将 Workers 与 KV 连接。

![](https://i2.wp.com/s3-jp-ap-3.040407.xyz/oss/photos/msedge_vIaafuvIAK.png)

回到上面，快速编辑里面编辑代码。

![](https://i2.wp.com/s3-jp-ap-3.040407.xyz/oss/photos/msedge_7h4KoaWu1v.png)

将 [本文件](https://github.com/LloydAsp/nfd/blob/main/worker.js) 内容全部复制即可。

```
const TOKEN = ENV_BOT_TOKEN // Get it from @BotFather
const WEBHOOK = '/endpoint'
const SECRET = ENV_BOT_SECRET // A-Z, a-z, 0-9, _ and -
const ADMIN_UID = ENV_ADMIN_UID // your user id, get it from https://t.me/username_to_id_bot

const NOTIFY_INTERVAL = 3600 * 1000;
const fraudDb = 'https://raw.githubusercontent.com/LloydAsp/nfd/main/data/fraud.db';
const notificationUrl = 'https://raw.githubusercontent.com/LloydAsp/nfd/main/data/notification.txt'
const startMsgUrl = 'https://raw.githubusercontent.com/LloydAsp/nfd/main/data/startMessage.md';

const enable_notification = true
/**
 * Return url to telegram api, optionally with parameters added
 */
function apiUrl (methodName, params = null) {
  let query = ''
  if (params) {
    query = '?' + new URLSearchParams(params).toString()
  }
  return `https://api.telegram.org/bot${TOKEN}/${methodName}${query}`
}

function requestTelegram(methodName, body, params = null){
  return fetch(apiUrl(methodName, params), body)
    .then(r => r.json())
}

function makeReqBody(body){
  return {
    method:'POST',
    headers:{
      'content-type':'application/json'
    },
    body:JSON.stringify(body)
  }
}

function sendMessage(msg = {}){
  return requestTelegram('sendMessage', makeReqBody(msg))
}

function copyMessage(msg = {}){
  return requestTelegram('copyMessage', makeReqBody(msg))
}

function forwardMessage(msg){
  return requestTelegram('forwardMessage', makeReqBody(msg))
}

/**
 * Wait for requests to the worker
 */
addEventListener('fetch', event => {
  const url = new URL(event.request.url)
  if (url.pathname === WEBHOOK) {
    event.respondWith(handleWebhook(event))
  } else if (url.pathname === '/registerWebhook') {
    event.respondWith(registerWebhook(event, url, WEBHOOK, SECRET))
  } else if (url.pathname === '/unRegisterWebhook') {
    event.respondWith(unRegisterWebhook(event))
  } else {
    event.respondWith(new Response('No handler for this request'))
  }
})

/**
 * Handle requests to WEBHOOK
 * https://core.telegram.org/bots/api#update
 */
async function handleWebhook (event) {
  // Check secret
  if (event.request.headers.get('X-Telegram-Bot-Api-Secret-Token') !== SECRET) {
    return new Response('Unauthorized', { status: 403 })
  }

  // Read request body synchronously
  const update = await event.request.json()
  // Deal with response asynchronously
  event.waitUntil(onUpdate(update))

  return new Response('Ok')
}

/**
 * Handle incoming Update
 * https://core.telegram.org/bots/api#update
 */
async function onUpdate (update) {
  if ('message' in update) {
    await onMessage(update.message)
  }
}

/**
 * Handle incoming Message
 * https://core.telegram.org/bots/api#message
 */
async function onMessage (message) {
  if(message.text === '/start'){
    let startMsg = await fetch(startMsgUrl).then(r => r.text())
    return sendMessage({
      chat_id:message.chat.id,
      text:startMsg,
    })
  }
  if(message.chat.id.toString() === ADMIN_UID){
    if(!message?.reply_to_message?.chat){
      return sendMessage({
        chat_id:ADMIN_UID,
        text:'使用方法，回复转发的消息，并发送回复消息，或者`/block`、`/unblock`、`/checkblock`等指令'
      })
    }
    if(/^\/block$/.exec(message.text)){
      return handleBlock(message)
    }
    if(/^\/unblock$/.exec(message.text)){
      return handleUnBlock(message)
    }
    if(/^\/checkblock$/.exec(message.text)){
      return checkBlock(message)
    }
    let guestChantId = await nfd.get('msg-map-' + message?.reply_to_message.message_id,
                                      { type: "json" })
    return copyMessage({
      chat_id: guestChantId,
      from_chat_id:message.chat.id,
      message_id:message.message_id,
    })
  }
  return handleGuestMessage(message)
}

async function handleGuestMessage(message){
  let chatId = message.chat.id;
  let isblocked = await nfd.get('isblocked-' + chatId, { type: "json" })
  
  if(isblocked){
    return sendMessage({
      chat_id: chatId,
      text:'Your are blocked'
    })
  }

  let forwardReq = await forwardMessage({
    chat_id:ADMIN_UID,
    from_chat_id:message.chat.id,
    message_id:message.message_id
  })
  console.log(JSON.stringify(forwardReq))
  if(forwardReq.ok){
    await nfd.put('msg-map-' + forwardReq.result.message_id, chatId)
  }
  return handleNotify(message)
}

async function handleNotify(message){
  // 先判断是否是诈骗人员，如果是，则直接提醒
  // 如果不是，则根据时间间隔提醒：用户id，交易注意点等
  let chatId = message.chat.id;
  if(await isFraud(chatId)){
    return sendMessage({
      chat_id: ADMIN_UID,
      text:`检测到骗子，UID${chatId}`
    })
  }
  if(enable_notification){
    let lastMsgTime = await nfd.get('lastmsg-' + chatId, { type: "json" })
    if(!lastMsgTime || Date.now() - lastMsgTime > NOTIFY_INTERVAL){
      await nfd.put('lastmsg-' + chatId, Date.now())
      return sendMessage({
        chat_id: ADMIN_UID,
        text:await fetch(notificationUrl).then(r => r.text())
      })
    }
  }
}

async function handleBlock(message){
  let guestChantId = await nfd.get('msg-map-' + message.reply_to_message.message_id,
                                      { type: "json" })
  if(guestChantId === ADMIN_UID){
    return sendMessage({
      chat_id: ADMIN_UID,
      text:'不能屏蔽自己'
    })
  }
  await nfd.put('isblocked-' + guestChantId, true)

  return sendMessage({
    chat_id: ADMIN_UID,
    text: `UID:${guestChantId}屏蔽成功`,
  })
}

async function handleUnBlock(message){
  let guestChantId = await nfd.get('msg-map-' + message.reply_to_message.message_id,
  { type: "json" })

  await nfd.put('isblocked-' + guestChantId, false)

  return sendMessage({
    chat_id: ADMIN_UID,
    text:`UID:${guestChantId}解除屏蔽成功`,
  })
}

async function checkBlock(message){
  let guestChantId = await nfd.get('msg-map-' + message.reply_to_message.message_id,
  { type: "json" })
  let blocked = await nfd.get('isblocked-' + guestChantId, { type: "json" })

  return sendMessage({
    chat_id: ADMIN_UID,
    text: `UID:${guestChantId}` + (blocked ? '被屏蔽' : '没有被屏蔽')
  })
}

/**
 * Send plain text message
 * https://core.telegram.org/bots/api#sendmessage
 */
async function sendPlainText (chatId, text) {
  return sendMessage({
    chat_id: chatId,
    text
  })
}

/**
 * Set webhook to this worker's url
 * https://core.telegram.org/bots/api#setwebhook
 */
async function registerWebhook (event, requestUrl, suffix, secret) {
  // https://core.telegram.org/bots/api#setwebhook
  const webhookUrl = `${requestUrl.protocol}//${requestUrl.hostname}${suffix}`
  const r = await (await fetch(apiUrl('setWebhook', { url: webhookUrl, secret_token: secret }))).json()
  return new Response('ok' in r && r.ok ? 'Ok' : JSON.stringify(r, null, 2))
}

/**
 * Remove webhook
 * https://core.telegram.org/bots/api#setwebhook
 */
async function unRegisterWebhook (event) {
  const r = await (await fetch(apiUrl('setWebhook', { url: '' }))).json()
  return new Response('ok' in r && r.ok ? 'Ok' : JSON.stringify(r, null, 2))
}

async function isFraud(id){
  id = id.toString()
  let db = await fetch(fraudDb).then(r => r.text())
  let arr = db.split('\n').filter(v => v)
  console.log(JSON.stringify(arr))
  let flag = arr.filter(v => v === id).length !== 0
  console.log(flag)
  return flag
}
```

修改后保存并部署即可。

然后访问 https://demo.demo.workers.dev/UUID 注册 WebSoket 即可。

私聊机器人，各项功能运行正常即可。

![](https://i2.wp.com/s3-jp-ap-3.040407.xyz/oss/photos/Telegram_8IcKciOFRj.png)