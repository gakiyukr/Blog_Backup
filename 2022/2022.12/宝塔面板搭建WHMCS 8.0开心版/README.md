## 前言

借着这篇文章，简单说说现在的中午互联网环境，一篇文章抄来抄去，一个人错了一群人都错；遍地都是的资源拿去倒卖，你自己破解的/做的，拿去卖钱无可厚非，不是自己做的资源，也拿去倒卖，并且价格高的离谱；动不动就关注公众号，加群获取解压密码。

CSDN、某某云开发者社区，各种奇葩文章，还有复制一阵子没把格式复制来的，链接丢了的，比比皆是。

## 下载链接

声明一下，里面有一份7.6的源码，一份8.0的源码，安装步骤一样的，没啥可说的。

7.6需要手动覆盖破解补丁，如果使用的我的7.6整合包则不需要，和8.0一个安装流程，两个的汉化补丁是通用的。

主题和插件，自己试试看能不能用，我不可能一个一个试。

[Gitlab](https://gitlab.com/gakiyukr/whmcs)

[Google Drive](https://drive.google.com/drive/folders/1YanQ_fPCSL30QwPtSuTLdFLnKh7IhoWF?usp=share_link)

OneDrive

## 环境准备

~~宝塔面板的正常建站环境~~ 废话

PHP需要7.4，8.0缺少一个解密扩展。安装下图的扩展。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-02_20-33-54.png)

## 安装

新建网站，数据库，没啥可说的。

将程序解压到目录，然后将 configuration.php.new 改成 configuration.php

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-02_21-35-02.png)

然后访问 网站域名/install，运行安装程序。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-02_21-37-28.png)

这里是配置检查，可以看到环境配置是否满足。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-02_21-38-17.png)

授权码可以瞎写，数据库配置按照你的实际情况来。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-02_21-39-33.png)

设置网站管理员密码

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-02_21-46-52.png)

这里需要将网站根目录的install文件夹删除，并且需要设置一个每五分钟执行一次的定时任务。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-02_21-46-01.png)

接下来就可以访问管理后台了。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-02_21-51-06.png)

后台全部是英文的，这里需要手动添加汉化补丁。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-02_21-51-41.png)

将汉化补丁放入 网站根目录/admin/lang/ 下。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-02_21-53-21.png)

过段时间刷新一下后台即可发现汉化已经生效

（鉴于这是多年前的汉化文件了，很多地方汉化不完整，搭配着浏览器翻译凑活着看）

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-02_21-56-03.png)

## 如何更换模板

以整合包提供的coowhm主题为例，将各自的文件夹内容放进各自的文件夹内。

coowhm-plus放入templates文件夹（一般来说只有这一步）ProductGroups.php放入./includes/hooks文件夹内。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-02_22-01-54.png)

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-02_22-02-54.png)

在后台设置启用新模板即可。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-02_22-06-54.png)