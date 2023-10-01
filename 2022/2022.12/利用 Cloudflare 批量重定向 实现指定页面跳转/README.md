批量重定向可以使得多个网站的，使用一套重定向请求，减少配置成本。并且由于重定向在Cloudflare边缘节点完成，减少了源站的压力。
前提：你的域名要接入在Cloudflare

批量重定向是一项全局设置，首先要去配置重定向规则，名称随便写，我的需求是大陆ip访问自带跳转至反诈页面，所以说名称我写做 chinaipban，类型选择重定向。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-20_08-43-43.png)

这里前面选择你的源站，后面选择你需要跳转到的网页，举个例子，我要把 [该网站](https://shop.avalonsky.cyou/) 跳转到 [电信的反诈页面](https://96110.pages.dev/Backup/ChinaTelecom/CT)

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-20_08-51-37.png)

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-20_08-58-29.png)

然后点击侧栏的批量重定向，创建一个重定向规则。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-20_08-59-57.png)

这个时候就是各位非常熟悉的防火墙规则了

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-20_09-21-26.png)

这里就可以根据自己的需求来了，如果你想屏蔽大陆ip，那么选择 国家/地区 等于 China。如果你想把他当跳转用，可以选择 国家/地区 不等于 朝鲜（因为并不会存在朝鲜IP访问我们的网站）即可做到所有访客跳转。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-20_09-31-21.png)