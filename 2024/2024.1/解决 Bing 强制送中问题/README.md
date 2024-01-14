## 什么是送中

微软在部分产品上提供的中国大陆特供版本，在功能上有或多或少的阉割。

## 具体表现

- Edge 的 Bing 搜索默认强制国区，无法通过网络环境的变化修改

- 搜索域名是 cn.bing.com

- Copilot（New Bing）不可用

- 安全搜索不可关闭

- 静默安装某些特色软件，例如微软电脑管家

## 如何查看自己是否为国区

  浏览器内打开 `edge://settings/searchEngines` 如果默认的 Bing 是 `{bing:cnBaseURL}` 则是国区特供。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/msedge_Ac61LVwoRQ.png)

## 解决方法

大前提：需要有合适的网络环境，如果用中国大陆 IP 访问 Bing，那么本文接下来的内容全都是在放屁。

早期版本是可以编辑搜索引擎的，后来的版本修复了这个 Bug。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/msedge_B3nHHt9qhW.png)

添加一个新搜索引擎，可以命名为 `Bing 国际版` ，捷径填写 `bing.com`，使用 URL %s 取代查詢填写 `{bing:baseURL}search?q=%s&{bing:cvid}{bing:msb}{google:assistedQueryStats}` 保存即可。

然后将该搜索引擎设置为默认搜索引擎即可。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/msedge_pA1aNPOO8D.png)

可以看到，设置后再去搜索，安全过滤也是可以关闭的。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/msedge_82HtNUO0iZ.png)

## 根治

来自 [微软的阴间活真的越来越多了 - V2EX](https://www.v2ex.com/t/944715) 可以自行查看。