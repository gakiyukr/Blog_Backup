## 速度测试

### Azure CDN

![](https://s3-jp-ap-3.040407.xyz/oss/photos/azcdntest191023.png)

### Jetpack CDN

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Jetpackcdntest191023.png)

## 介绍

Jetpack 是 WordPress.com 旗下的产品。

Jetpack Site Accelerator（又叫 Jetpack CDN ）可以使用 Jetpack 的全球网络优化图片以及静态文件加载速度。

（WP 后台的 Jetpack 插件和本文差不多是一个东西）

## 加速域名

i0.wp.com
i1.wp.com
i2.wp.com
i3.wp.com

## 使用方法

```
https://i {0,1,2,3}.wp.com/图片原URL
```

例：

原始地址：https://donate.amex.my.id/static/img/logo/Alipay_HKMO_Logo.webp

加速后地址：https://i0.wp.com/donate.amex.my.id/static/img/logo/Alipay_HKMO_Logo.webp

![](https://i0.wp.com/donate.amex.my.id/static/img/logo/Alipay_HKMO_Logo.webp)

## 支持格式

gif、png、webp、jpeg 、jpg

## 优势

- 目前看起来，免费，储存时间为永久
- 支持 SSL 访问
- 国内访问速度不错，除了部分地区被劫持
- 多个域可做负载均衡

## 劣势

- 永久储存，所以一经上传则无法删除
- 不支持大于 55M 的图片
- 在某些情况下，会压缩原始图片
- 原图片有防盗链会导致失败
- 官方如发现有滥用会删除图片加速，域名会加入黑名单

## 高级参数用法
支持 URL 直接传参，支持图片尺寸进行修改，调整图片亮度，滤镜，质量等等

![](https://i2.wp.com/s3-jp-ap-3.040407.xyz/oss/photos/msedge_KsfvxH7IUs.png)
[更多参数说明](https://developer.wordpress.com/docs/site-accelerator/site-accelerator-api/)

## 总结

建议用于做自己图床的备份。还是要多种方式备份图片，以防万一！！

本站自从本文后的所有文章，均采用了这种方法备份图片。

## 鸣谢

本文部分内容借鉴于 [WordPress携手Jetpack免费提供图片CDN加速，永久缓存！ - 如有乐享 (ruyo.net)](https://51.ruyo.net/18486.html)