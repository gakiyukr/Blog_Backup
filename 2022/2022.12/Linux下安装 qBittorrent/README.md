qBittorrent 是一个支持多平台的 BT 下载工具。qBittorrent 的软件界面虽然是用 QT 开发的，但 qBittorrent 也包含一个 WebUI，可以通过浏览器远程管理，没有图形界面的设备也可以使用。

## 安装

这里使用一键脚本安装：

脚本仓库地址：[传送门](https://github.com/Aniverse/qbittorrent-nox-static)

首先下载脚本：

```
wget https://github.com/Aniverse/qbittorrent-nox-static/raw/master/install.sh
```

然后运行

```
bash install.sh -u 用户名 -p 密码 -w 端口 -v 版本
```

将变量替换为自己的设置，示例：

```
bash install.sh -u admin -p 123456 -w 8080 -v 4.3.0.lt.1.2.10
```

其他版本可以在作者的 [sourceforge](https://sourceforge.net/projects/inexistence/files/qbittorrent/) 找到。

然后运行qBittorren

```
qbittorrent-nox
```

第一次运行会提示法律声明，输入Y确认。

```
root@linux:~# qbittorrent-nox

*** Legal Notice ***
qBittorrent is a file sharing program. When you run a torrent, its data will be made available to others by means of upload. Any content you share is your sole responsibility.

No further notices will be issued.

Press 'y' key to accept and continue...
y
"Web UI: Unable to bind to IP: *, port: 8080. Reason: The bound address is already in use"
```

然后就可以访问WebUI了。

## WebUI配置

没有特殊情况下，UI应该是中文，如果非中文可以自行修改。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-09_14-19-48.png)

如果是用于BT下载，可以手动添加一些 Tracker，否则一些比较冷门的资源可能没速度。

具体的 Tracker 列表可以去[XIU2/TrackersListCollection: 🎈 Updated daily! A list of popular BitTorrent Trackers! / 每天更新！全网热门 BT Tracker 列表！ (github.com)](https://github.com/XIU2/TrackersListCollection) 找找看。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-09_14-23-54.png)