## 前言

东西确实是好东西，三网强制4837回程，就是价格略微有点贵，最便宜也需要50CNY/m。最低配拿去搞个小站还是可以的，只用来科学上网就太奢侈了。

![Snipaste_01-31_15-45-03](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_01-31_15-45-03.png)

丢一个aff，我可以拿到10%的提成：[https://idc.wiki/aff.php?aff=2783](https://idc.wiki/aff.php?aff=2783)

无aff传送门：[https://idc.wiki](https://idc.wiki/)

## 配置测试

```
-------------------- A Bench Script By spiritlhl ---------------------
                   测评频道: https://t.me/vps_reviews                    
版本：2023.01.20
更新日志：融合怪九代目(集合百家之长)(专为测评频道小鸡而生)
-----------------感谢teddysun和superbench和yabs开源-------------------
 CPU 型号          : AMD Ryzen 9 5900X 12-Core Processor
 CPU 核心数        : 1
 CPU 频率          : 3697.908 MHz
 CPU 缓存          : 512 KB
 硬盘空间          : 49.3 GB (5.0 GB 已用)
 内存              : 976 MB (262 MB 已用)
 Swap              : 1024 MB (20 MB 已用)
 系统在线时间      : 0 days, 0 hour 31 min
 负载              : 0.11, 0.39, 0.35
 系统              : Ubuntu 20.04.5 LTS
 AES-NI指令集      : ✔ Enabled
 VM-x/AMD-V支持    : ✔ Enabled
 架构              : x86_64 (64 Bit)
 内核              : 5.4.0-120-generic
 TCP加速方式       : bbr
 虚拟化架构        : KVM
 ASN组织           : AS40065 CNSERVERS LLC
 位置              : Los Angeles / US
 地区              : California
-------------------CPU测试--感谢lemonbench开源------------------------
 -> CPU 测试中 (Fast Mode, 1-Pass @ 5sec)
 1 线程测试(1核)得分:           4936 Scores
-------------------内存测试--感谢lemonbench开源-----------------------
 -> 内存测试 Test (Fast Mode, 1-Pass @ 5sec)
 单线程读测试:          54408.82 MB/s
 单线程写测试:          27866.29 MB/s
----------------磁盘IO读写测试--感谢lemonbench开源--------------------
 -> 磁盘IO测试中 (4K Block/1M Block, Direct Mode)
 测试操作               写速度                                  读速度
 100MB-4K Block         77.8 MB/s (0.05 IOPS, 1.35s))           109 MB/s (26508 IOPS, 0.97s)
 1GB-1M Block           1.3 GB/s (1245 IOPS, 0.80s)             2.8 GB/s (2671 IOPS, 0.37s)
-------------------磁盘IO读写测试--感谢yabs开源-----------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 231.39 MB/s  (57.8k) | 1.15 GB/s    (18.0k)
Write      | 232.00 MB/s  (58.0k) | 1.15 GB/s    (18.1k)
Total      | 463.40 MB/s (115.8k) | 2.31 GB/s    (36.1k)           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 1.40 GB/s     (2.7k) | 1.50 GB/s     (1.4k)
Write      | 1.48 GB/s     (2.8k) | 1.60 GB/s     (1.5k)
Total      | 2.89 GB/s     (5.6k) | 3.11 GB/s     (3.0k)
--------------------流媒体解锁--感谢sjlleo开源------------------------
以下测试的解锁地区是准确的，但是不是完整解锁的判断可能有误，这方面仅作参考使用
Youtube
[IPv4]
连接方式: Youtube Video Server
视频缓存节点地域: 美国  洛杉机(LAX31S13)
Youtube识别地域: 无信息(null)
Netflix
[IPv4]
您的出口IP可以使用Netflix，但仅可看Netflix自制剧
NF所识别的IP地域信息：美国
[IPv6]
您的网络可能没有正常配置IPv6，或者没有IPv6网络接入
DisneyPlus
[IPv4]
当前IPv4出口解锁DisneyPlus
区域：美国区
解锁Youtube，Netflix，DisneyPlus上面和下面进行比较，不同之处自行判断
---------------流媒体解锁--感谢RegionRestrictionCheck开源-------------
 以下为IPV4网络测试，若无IPV4网络则无输出
============[ Multination ]============
 Dazn:                                  No
 HotStar:                               Yes (Region: US)
 Disney+:                               No
 Netflix:                               Originals Only
 YouTube Premium:                       Yes
 Amazon Prime Video:                    Yes (Region: US)
 TVBAnywhere+:                          Yes
 iQyi Oversea Region:                   US
 Viu.com:                               No
 YouTube CDN:                           Los Angeles, CA 
 Netflix Preferred CDN:                 Chicago, IL  
 Spotify Registration:                  No
 Steam Currency:                        USD
=======================================
 以下为IPV6网络测试，若无IPV6网络则无输出
-------------TikTok解锁--感谢lmc999加密脚本及fscarmen PR--------------
 Tiktok Region:         【US】
-----------------欺诈分数以及IP质量检测--本频道原创-------------------
以下仅作参考，不代表100%准确，如果和实际情况不一致请手动查询多个数据库比对
------以下为IPV4检测------
scamalytics数据库:
ip-api数据库:
  手机流量: No
  代理服务: No
  数据中心: Yes
abuseipdb数据库-abuse得分： 0
IP类型:
  IP2Location数据库:  Data Center/Web Hosting/Transit
  liveipmap数据库：(DCH) Data Center/Web Hosting/Transit
  ping0数据库: IDC机房IP CN2线路
Google搜索可行性：YES
-----------------三网回程--感谢zhanghanyun/backtrace开源--------------
2023/01/27 10:03:08 北京电信 219.141.136.12  联通4837[普通线路]           
2023/01/27 10:03:08 北京联通 202.106.50.1    联通4837[普通线路]           
2023/01/27 10:03:08 北京移动 221.179.155.161 联通4837[普通线路]           
2023/01/27 10:03:08 上海电信 202.96.209.133  联通4837[普通线路]           
2023/01/27 10:03:08 上海联通 210.22.97.1     联通4837[普通线路]           
2023/01/27 10:03:08 上海移动 211.136.112.200 联通4837[普通线路]           
2023/01/27 10:03:08 广州电信 58.60.188.222   联通4837[普通线路]           
2023/01/27 10:03:08 广州联通 210.21.196.6    联通4837[普通线路]           
2023/01/27 10:03:08 广州移动 120.196.165.24  联通4837[普通线路]           
2023/01/27 10:03:08 成都电信 61.139.2.69     联通4837[普通线路]           
2023/01/27 10:03:08 成都联通 119.6.6.6       联通4837[普通线路]           
2023/01/27 10:03:08 成都移动 211.137.96.205  联通4837[普通线路]           
------------------回程路由--感谢fscarmen开源及PR----------------------
IPv4 ASN: Multacom Corporation
依次测试电信，联通，移动经过的地区及线路，核心程序来由: ipip.net ，请知悉!
广州电信 58.60.188.222
0.37 ms  AS40065  美国, 加利福尼亚州, 洛杉矶, ceranetworks.com
0.31 ms  AS40065  美国, 加利福尼亚州, 洛杉矶, ceranetworks.com
0.52 ms  *  局域网
156.90 ms  AS40065  美国, 加利福尼亚州, 洛杉矶, ceranetworks.com
166.52 ms  AS4837  中国, 上海, chinaunicom.com, 联通
161.86 ms  AS4837  中国, 上海, chinaunicom.com, 联通
161.71 ms  AS4837  中国, 上海, chinaunicom.com, 联通
171.00 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
167.51 ms  AS4134  中国, 广东, 广州, chinatelecom.com.cn, 电信
168.42 ms  AS4134  中国, 广东, 深圳, chinatelecom.com.cn, 电信
167.82 ms  AS4134  中国, 广东, 深圳, chinatelecom.com.cn, 电信
广州联通 210.21.196.6
0.39 ms  AS40065  美国, 加利福尼亚州, 洛杉矶, ceranetworks.com
0.48 ms  *  局域网
152.82 ms  AS40065  美国, 加利福尼亚州, 洛杉矶, ceranetworks.com
158.28 ms  AS4837  中国, 上海, chinaunicom.com, 联通
157.64 ms  AS4837  中国, 上海, chinaunicom.com, 联通
161.82 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
166.54 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
广州移动 120.196.165.2
0.48 ms  AS40065  美国, 加利福尼亚州, 洛杉矶, ceranetworks.com
0.31 ms  AS40065  美国, 加利福尼亚州, 洛杉矶, ceranetworks.com
0.49 ms  *  局域网
151.09 ms  AS40065  美国, 加利福尼亚州, 洛杉矶, ceranetworks.com
159.98 ms  AS4837  中国, 上海, chinaunicom.com, 联通
160.84 ms  AS4837  中国, 上海, chinaunicom.com, 联通
157.28 ms  AS4837  中国, 上海, chinaunicom.com, 联通
158.85 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
160.07 ms  AS56040  中国, 广东, 深圳, chinamobile.com, 移动
--------网络测速--由teddysun和superspeed开源及spiritlhls整理----------
测速点位置       上传速度        下载速度        延迟
Speedtest.net    910.71 Mbps     665.82 Mbps     6.03 ms
洛杉矶           1993.94 Mbps    2038.17 Mbps    1.94 ms
新加坡           459.53 Mbps     1507.41 Mbps    187.92 ms
中国香港         514.27 Mbps     964.69 Mbps     168.00 ms
电信上海         440.69 Mbps     928.52 Mbps     132.92 ms
电信广东广州5G   216.67 Mbps     1488.53 Mbps    158.06 ms
联通上海         514.94 Mbps     1699.78 Mbps    160.02 ms
联通湖南长沙     545.31 Mbps     1705.47 Mbps    151.98 ms
移动广西南宁     870.44 Mbps     938.32 Mbps     64.94 ms
----------------------------------------------------------------------
 总共花费      : 6 分 22 秒
 时间          : Fri Jan 27 10:08:17 UTC 2023
----------------------------------------------------------------------
```

