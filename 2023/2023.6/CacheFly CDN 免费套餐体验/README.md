CacheFly 近日宣布了提供免费 CDN 套餐，最近在站长圈还是有点热度的，这里也就水一篇文章，简单测评一下这个 CDN。

[官网](https://www.cachefly.com/)

[注册链接](https://portal.cachefly.com/signup/free2023)

## 前提

免费归免费，但是要绑卡。仅验证不扣费，所以说还是有一定的操作空间的。

**不建议绑定自己的实体卡，不建议绑定国内卡，更不建议绑定有透支额度的信用卡，被刷房子易主。**

## 免费套餐

- 节点：北美+欧洲
- 流量：5 TB
- 超出流量：0.05 USD/GB
- 自定义域名：1个
- 支持SSL：需自行上传
- WebSockets：不支持

不支持 WebSockets，所以想拿去玩骚操作的可以洗洗睡了。

这家的付费套餐不用想，295 USD/月，压根就不做个人业务。

## 配置网站

注册没啥可说的，用户名邮箱密码，绑卡即可。这里直接讲如何配置网站。

完成注册后，会创建一个以你的用户名为名称的项目，点击 `Use Configuration Wizard` 开始最基础的配置。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_06-29_17-02-52.png)

填写源站地址，这里只能是域名，不能是 IP，所以说需要解析上去一个域名才能用。

下方可以选择使用 HTTP/HTTPS 协议。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_06-29_17-04-17.png)

接下来设置域名，也可以选择不使用自定义域名，而使用他给的 CNAME 域名。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_06-29_17-04-17.png)

然后上传自定义 SSL 证书，建议上传一个长期的，例如 1年 180天 等等。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_06-29_17-10-59.png)

前面是证书，后面是公钥，添加好下一步即可。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_06-29_17-11-18.png)

然后将你的自定义域名，CNAME 到平台提供的域名即可。





## 速度测试

这是几个我分别部署在不同平台，使用不同的 CDN 的测试网站：

[Cloudflare](https://911.amex.my.id/CN/CU/)

[Cachefly](https://96110.amex.my.id/CN/CU/)

[Vercel](https://global.dmz-wiki.amex.my.id/)

以及本站使用的是 Azure CDN。

可以自行去测试平台测试国内加载速度。

Cachefly 自定义域名：

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Cachefly-zdy.png)

Cachefly CNAME 域名：

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Cachefly-cname.png)

Cloudflare CDN：

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Cloudflare.png)

Vercel 自带 CDN：

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Vercel.png)

Azure CDN：

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Azure-CDN.png)

从纸面数据来说，这四家的大体速度都是差不多的。

整体上来说，CacheFly 在免费 CDN 中还是不错的，尤其是 Azure 无法白嫖，Vercel 无法自由使用，Cloudflare 被某些地方的某些运营商屏蔽的大环境中，虽然只提供了欧美接入点，但是最终表现还是能对得起免费的水平。

## 高级功能

免费版不提供某些高级功能，如 WebSockets、DDOS 防护 等。

这里也就不做演示了，请自行研究其他功能。

## 总结

如果你当地 Cloudflare 被干扰的厉害，那么用 CacheFly 还是不错的，5 TB 流量足够小型站点使用。

个人观点认为，不支持 WebSockets 是一种明智的做法，Cloudflare、Gcore、AWS CFT 都是因为被拿去乱搞玩废的。

最后还是那句话：

**不建议绑定自己的实体卡，不建议绑定国内卡，更不建议绑定有透支额度的信用卡，被刷房子易主。**

**不建议绑定自己的实体卡，不建议绑定国内卡，更不建议绑定有透支额度的信用卡，被刷房子易主。**

**不建议绑定自己的实体卡，不建议绑定国内卡，更不建议绑定有透支额度的信用卡，被刷房子易主。**

