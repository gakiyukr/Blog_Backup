ACME是一个一键签发SSL证书的脚本，可以通过DNS服务商的API进行自动续期，也可以签发通配符、多域名证书等大部分免费证书不提供的服务。

## 安装ACME

```
wget https://get.acme.sh -O install_acme.sh
chmod +x install_acme.sh
./install_acme.sh email=你自己的邮箱
```

## 修改签发机构

ACME默认的SSL签发者是ZeroSSL，如果需要可以修改到BuyPass、Let's Encrypt等，不过个人建议用ZeroSSL，Let's Encrypt更换新根证书以后，存在部分老设备无法访问的问题。

切换 Let's Encrypt

```bash
acme.sh --set-default-ca --server letsencrypt
```

切换 Buypass

```bash
acme.sh --set-default-ca --server buypass
```

切换 ZeroSSL（注：这玩意官网不支持泛域名，多域名啥的，但是ACME是支持的）

```bash
acme.sh --set-default-ca --server zerossl
```

切换 [SSL.com](http://ssl.com/)

```bash
acme.sh --set-default-ca --server ssl.com
```

切换 Google Public CA（Google需要自己按照[官方博客](https://cloud.google.com/blog/products/identity-security/automate-public-certificate-lifecycle-management-via--acme-client-api)的教程去申请API，并且这玩意因为某些众所周知的问题，国内机器申请是无法连接到验证域名的）

```bash
acme.sh --set-default-ca --server google
```

| 功能       | LE   | Buypass | ZeroSSL | SSL.com | Google Public CA |
| ---------- | ---- | ------- | ------- | ------- | ---------------- |
| 有效期     | 90   | 180     | 90      | 90      | 90               |
| 多域名     | √    | 5 个    | √       | √，收费 | √                |
| 泛域名     | √    | ×       | √       | √，收费 | √                |
| Rate Limit | √    | √       | ×       | 未知    | √                |
| GUI 管理   | ×    | ×       | √       | √       | ×                |
| ECC 证书链 | ×    | ×       | √       | 未知    | ×                |

## 通过DNS服务商API自动申请

然后进入安装文件夹，设定CF API变量：

```
cd ~/.acme.sh
export CF_Key="全局API Key"
export CF_Email="登录邮箱"
如果你认为使用有风险，那么可以使用Zone API：
export CF_Token="复制下来的 Token"
export CF_Account_ID="复制下来的 Account ID"
export CF_Zone_ID="复制下来的 Zone ID"
```

ACME也支持其他的DNS服务商，如阿里、腾讯（但是不支持华为，下面还有曲线救国的方法）其他API的设置，可以参考[官方文档](https://github.com/acmesh-official/acme.sh/wiki/dnsapi)。

然后，我们就可以使用以下的命令，去签发SSL了。最后面的参数cf代表使用Cloudflare的API，其他运营商参考官方文档。

如果要签发单域名证书，可以使用：

```
/root/.acme.sh/acme.sh --issue -d test.demo.com --dns dns_cf
```

如果要签发泛域名证书，记得需要同时添加 demo.com和*.demo.com。

```
/root/.acme.sh/acme.sh --issue -d demo.com -d *.demo.com --dns dns_cf
```

ACME也支持签发多域名证书，可以使用：

```
/root/.acme.sh/acme.sh --issue -d demo.com -d demo1.com --dns dns_cf
```

## 通过CNAME别名曲线救国

前面说到，ACME不支持华为云，那么这里我们可以曲线救国，前提是你需要有一个域名接入在ACME支持DNS的服务商，并且不能是tk cf ml这种域名。

例如我有个user.edu接入在华为云，有个96110.xyz接入在Cloudflare，那么现在需要解析一条CNAME记录。

_acme-challenge.user.edu ->CNAME到-> _acme-challenge.96110.xyz

然后使用下面的命令：

```
/root/.acme.sh/acme.sh --issue -d user.edu -d *.user.edu --challenge-alias 96110.xyz --dns dns_cf
```

即可到达曲线救国，通过自动申请证书，并且可以自动续期。

## 其他申请方法

ACME也可以使用HTTP验证，或者是80端口验证，但是鉴于这种方法不太好用，这里不做介绍了。

## 安装证书

ACME文件夹内有以域名命名的文件夹，里面有一堆文件，其中.key文件可以直接填到宝塔的密钥里，.cre文件可以填到宝塔的公钥里面。

## 其他命令

ACME更新频繁，建议开启自动更新。

```
/root/.acme.sh/acme.sh  --upgrade  --auto-upgrade #开启自动更新
/root/.acme.sh/acme.sh --upgrade  --auto-upgrade  0 #关闭自动更新
```

