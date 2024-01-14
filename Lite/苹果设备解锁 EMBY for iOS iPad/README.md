## 前言

EMBY for iOS 是需要付费的（5 USD 左右），否则就只能用 Web 版。本文通过 iOS/iPad 的网络工具解锁 EMBY 客户端，解决该问题。

**有条件请支持正版！！！**

**有条件请支持正版！！！**

**有条件请支持正版！！！**

PS：需要手动开启 HTTPS 解密/MitM，各软件方法不同，请自行解决。

## Shadowrocket

在配置文件的最下面，加入下面的两条规则即可。可以根据自己的网络情况选择。

GitHub 源：

```
[Script]
EmbyPremiere = type=http-response,script-path=https://raw.githubusercontent.com/rartv/SurgeScript/main/EmbyPremiere/EmbyPremiere.js,pattern=^https?:\/\/mb3admin.com\/admin\/service\/registration\/validateDevice,max-size=131072,requires-body=true,timeout=10,enable=true

[MITM]
hostname = mb3admin.com
```

GitLab 源：

```
[Script]
EmbyPremiere = type=http-response,script-path=https://gitlab.com/iptv-org/embypublic/-/raw/master/Script/EmbyPremiere.js,pattern=^https?:\/\/mb3admin.com\/admin\/service\/registration\/validateDevice,max-size=131072,requires-body=true,timeout=10,enable=true

[MITM]
hostname = mb3admin.com
```

原作者脚本仓库：[rartv/SurgeScript: My Surge Script (github.com)](https://github.com/rartv/SurgeScript) [TV / EmbyPublic · GitLab](https://gitlab.com/iptv-org/embypublic/)

## Loon

插件地址：`https://yfamily.vercel.app/plugin/Emby.plugin`

## Surge

导入模块即可：

GitHub 源：`https://raw.githubusercontent.com/rartv/SurgeScript/main/EmbyPremiere/EmbyPremiere.sgmodule`

GitLab 源：`https://gitlab.com/iptv-org/embypublic/-/raw/master/Script/EmbyPremiere.sgmodule`

## 其他 APP 解锁方案

其他 APP 我都没用过，因此没得写。

网上同类教程一模一大把，可以自行查找。