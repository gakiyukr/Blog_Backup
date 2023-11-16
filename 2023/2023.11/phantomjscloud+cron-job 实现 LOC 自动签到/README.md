

最近 LOC 开放注册，新涌入了不少 MJJ 。这里引用 LOC 的一个贴子，介绍一个自动签到每日获取积分的方法。

## 原理

使用 phantomjscloud ，自动登录 LOC，访问其他 MJJ 的个人空间。

使用 cron-job.org 每日定时执行。

本方法无需每天开电脑，一次配置，一劳永逸。

## 步骤

前往 [phantomjscloud.com](https://phantomjscloud.com/) 先去注册个账号

![](https://s3-jp-ap-3.040407.xyz/oss/photos/msedge_cyF0jcjbkL.png)

完成邮箱验证，获取到 API Key 保留备用。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/msedge_ptLhwuuUWT.png)

访问 [sandbox.onlinephpfunctions.com](https://sandbox.onlinephpfunctions.com/code/58d44bdc19a7fcfdf22b87d23cc902e8061a90a5) ，修改本脚本的第 4 7 8 行，分别改为你自己的数据即可。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/msedge_jHyJ5z63mq.png)

点击下面的“Execute code”，将下面生成的一个网址保存下来备用。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/msedge_foQ0XpXOfz.png)

这个时候可以使用自己的 VPS/软路由，写一个 Crontab 定时任务来定期 Curl/Wget 该链接。

也可以使用第三方服务来定期触发。

前往 [console.cron-job.org](https://console.cron-job.org/dashboard) 注册一个账号

默认的时区不是北京时间，自行去修改一下即可。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/msedge_XdhPziBSib.png)

添加一个新的定时工作，网址写刚刚获取到的那一串网址，设定一个合适的触发时间即可。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/msedge_n6zLZJzPMu.png)

可以点击下面的测试，看看是否成功。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/msedge_CS4MOBRW1O.png)

测试完成以后，可以顺便去论坛看看积分是否到账。

## 其他办法

[hostloc签到Python脚本 之 小鸡部署篇](https://hostloc.com/thread-846692-1-1.html)

[hostloc签到Python脚本 之 docker 篇](https://hostloc.com/forum.php?mod=redirect&goto=findpost&ptid=846520&pid=10397101) 

[hostloc签到Python脚本 之 Heroku 篇](https://hostloc.com/forum.php?mod=redirect&goto=findpost&ptid=846520&pid=10398510) 

[hostloc签到脚本 之 HTML+JS 及 PHP 篇](https://hostloc.com/thread-847005-1-1.html)

[hostloc签到Python脚本 之 云函数 篇](https://hostloc.com/thread-847567-1-1.html) 

[hostloc签到Go脚本 之 云函数 篇](https://hostloc.com/thread-848916-1-1.html)

[hostloc签到脚本 之 油猴脚本 篇](https://hostloc.com/thread-847601-1-1.html)

[hostloc签到JS脚本 之 浏览器 篇](https://hostloc.com/thread-848789-1-1.html)

[hostloc签到脚本 之 phantomjscloud 篇](https://hostloc.com/thread-848822-1-1.html) 

## 鸣谢

[【0527更新】不需要VPS、不需要开电脑，无感知自动定时签到~-美国VPS综合讨论-全球主机交流论坛 - Powered by Discuz! (hostloc.com)](https://hostloc.com/thread-848822-1-1.html)
