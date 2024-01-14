## 什么是 Telegram MTProto Proxy

TG 自主研发的专用代理，特点是跨平台，只要能装 TG 的设备都能用，包括且不限于电视盒子，车机，手表。（我自己就是在手表上用）

缺点：已经被识别了，比 HTTP/Socks5 安全，就是有可能天天被墙罢了。

## 安装

绿色版，需要先创建一个文件夹用于存放文件。

```
mkdir /home/mtproxy && cd /home/mtproxy
curl -s -o mtproxy.sh https://raw.githubusercontent.com/ellermister/mtproxy/master/mtproxy.sh && chmod +x mtproxy.sh && bash mtproxy.sh
```

## 使用方式

```
运行服务
bash mtproxy.sh start
调试运行
bash mtproxy.sh debug
停止服务
bash mtproxy.sh stop
重启服务
bash mtproxy.sh restart
```

## 卸载

绿色版，直接删掉文件夹即可。

## 优化

如果你所配置的代理需要公开分享或者给大量人使用，建议修改一下配置，防止报错。

编辑文件 `vi /etc/security/limits.conf  ` 在文件尾或者对应段加入内容，对用户级进行配置

```
soft nofile 655350
hard nofile 655350
```

表示对任何用户的软硬限制提升到 655350 个



接下来对系统级进行配置，`vi /etc/sysctl.conf` 加入配置。

```
fs.file-max = 655350
```

用户打开的最大文件描述符总数不会超过系统级的总数。

将内核参数生效

```
sysctl -p
```

