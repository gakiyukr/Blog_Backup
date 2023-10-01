## 前言

本教程只适用于有外挂字幕的视频，而并非硬字幕，也就是除了视频文件，还要有字幕文件，岛国小电影只有语音那种和本文不是一种东西。字幕文件一般来说是 SRT 格式。

顺手提一句，播放器个人建议使用 PotPlayer ，下文的字幕自动翻译也是基于 PotPlayer 进行的。

**PotPlayer**的官网是 [Global Potplayer (daum.net)](https://potplayer.daum.net/)，是韩国最大的门户网站之一 Daum 的产品，域名也是 Daum 的子域名，该网站在中国大陆被屏蔽，所以去百度、Bing 等地使用中文搜索，大概率搜到一堆某某下载站的垃圾东西。

## PotPlayer 实时字幕翻译

PotPlayer 自带了实时翻译的功能，默认自带 Google、Bing、Yandex、Naver 的翻译接口，填入相关的 API 即可使用。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_05-20_15-03-55.png)

也可以手动安装其他翻译软件的插件，个人感觉 DeepL 的翻译结果还是很不错的。

[DeepL 插件 Github 仓库传送门](https://github.com/Ermaotie/SubtitleTranslate_DeepL)

[百度翻译插件 Github 仓库传送门](https://github.com/fjqingyou/PotPlayer_Subtitle_Translate_Baidu)

上面的是作者仓库，为了防止意外，我备份了一份在 Gitlab 中。

[本人 Gitlab 仓库备份](https://gitlab.com/gakiyukr/potplayer-translate/)

使用的时候，将 `.as` 和 `.ico` 这两个文件丢到 PotPlayer 安装目录的 `Extension\Subtitle\Translate` 这个路径下即可。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_05-20_15-22-10.png)

DeepL 需要绑定支付方式，然后才可以使用 API Free，每个月 500000 （50万）字符基本上够用了，实在不行多开几个号也是可以的。Pro 看需求，量上去了这个加个还是不错的。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_05-20_15-23-24.png)

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_05-20_15-24-04.png)

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_05-20_15-24-17.png)

找到你的 API 密钥，填入 PotPlayer 即可，设置一下源语言等。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_05-20_15-27-05.png)

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_05-20_15-26-45.png)

## Tern-字幕组机翻小助手

这是另一个不错的翻译工具，他是一口气翻译出来，生成翻译后的文件，并非在视频播放的时候实时翻译，该工具支持的翻译服务商更多，例如 阿里、腾讯、Azure、AWS 等。

这个只有在线版可以使用 DeepL API，本地版是通过模拟浏览器运行使用 DeepL 网页版进行翻译的。

[Github 仓库](https://github.com/1c7/Translate-Subtitle-File)

[在线版](https://tern.1c7.me/#/)

[本地版](https://github.com/1c7/Translate-Subtitle-File/releases)

官方给出了非常详细的各个服务商 API 配置教程，这里就不多说了。

## 翻译效果测试

这里用的是 浪漫医生金师傅3 第三季的英文字幕，分别使用 Azure、AWS、DeepL 翻译，源文件和翻译结果均已上传到上文的 Gitlab 仓库中，可以自行查看。

个人体验，三家都大差不差，人名、地名、专有名词翻译的一塌糊涂按表不谈，都翻译的完全不符合中文使用习惯，或者是不符合语言逻辑，像极了我们一个一个单词往外蹦的中式英语。本身就是图一乐呵的水平，配合着画面知道讲了个什么事情，不至于和看哑剧一样两眼一抹黑，但是想要深入的理解故事，或者是体现出原句的水平，就不太现实了。

例如第258 259句，根据上下文和画面，能得知是这个运动员装病，结果都翻译成了伪造。

```
258
00:17:18,923 --> 00:17:21,675
这不是什么大事。这是一种常见的疾病
It's nothing big. It's a common illness

259
00:17:22,259 --> 00:17:23,259
称为伪造。
called faking.
```

整体上看，DeepL 还是胜过剩下两家的，AWS Azure 把“胃疼”翻译成了“我的胃要杀了我”，还是非常搞笑的。

## 后记

前段时间有人做出来了 OpenAI 翻译书籍，那么不知道有无大佬能做一个 OpenAI 翻译字幕的接口，从电子书来说，OpenAI 的翻译效果还是不错的。