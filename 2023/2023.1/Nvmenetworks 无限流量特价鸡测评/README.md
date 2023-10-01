## 前言

这破玩意及其灵车，随说价格便宜，但是这玩意能灵到邮件里的网站，域名都被卖了，~~并且管理后台还是个IP（SSL也是坏的），这两天刚修好。~~这两天MJJ拿去剑皇vscode，给母鸡搞炸了，隔三岔五就要去后台重启。速度也不怎么样，不拿去搬文件就没啥买的意义了。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_01-18_15-48-42.png)

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_01-18_15-50-01.png)

## 配置测试

```
-------------------- A Bench Script By spiritlhl ---------------------
                   测评频道: https://t.me/vps_reviews                    
版本：2023.01.07
更新日志：融合怪九代目(集合百家之长)(专为测评频道小鸡而生)
-----------------感谢teddysun和misakabench和yabs开源------------------
 CPU 型号          : AMD Ryzen 9 5950X 16-Core Processor
 CPU 核心数        : 1
 CPU 频率          : 4990.624 MHz
 CPU 缓存          : 512 KB
 硬盘空间          : 25.0 GB (2.0 GB 已用)
 内存              : 943 MB (152 MB 已用)
 Swap              : 0 MB (0 MB 已用)
 系统在线时间      : 0 days, 0 hour 13 min
 负载              : 0.02, 0.08, 0.11
 系统              : Debian GNU/Linux 11 (bullseye)
 AES-NI指令集      : ✔ Enabled
 VM-x/AMD-V支持    : ✔ Enabled
 架构              : x86_64 (64 Bit)
 内核              : 5.10.0-10-amd64
 TCP加速方式       : cubic
 虚拟化架构        : KVM
 ASN组织           : AS210912 Twistic Limited
 位置              : Berlin / DE
 地区              : Berlin
-------------------CPU测试--感谢lemonbench开源------------------------
 -> CPU 测试中 (Fast Mode, 1-Pass @ 5sec)
 1 线程测试(1核)得分:           4886 Scores
-------------------内存测试--感谢lemonbench开源-----------------------
 -> 内存测试 Test (Fast Mode, 1-Pass @ 5sec)
 单线程读测试:          56140.79 MB/s
 单线程写测试:          29195.99 MB/s
----------------磁盘IO读写测试--感谢lemonbench开源--------------------
 -> 磁盘IO测试中 (4K Block/1M Block, Direct Mode)
 测试操作               写速度                                  读速度
 100MB-4K Block         66.9 MB/s (0.06 IOPS, 1.57s))           82.5 MB/s (20140 IOPS, 1.27s)
 1GB-1M Block           1.9 GB/s (1856 IOPS, 0.54s)             2.3 GB/s (2210 IOPS, 0.45s)
-------------------磁盘IO读写测试--感谢yabs开源-----------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 359.61 MB/s  (89.9k) | 2.22 GB/s    (34.7k)
Write      | 360.56 MB/s  (90.1k) | 2.23 GB/s    (34.9k)
Total      | 720.17 MB/s (180.0k) | 4.45 GB/s    (69.6k)           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 2.46 GB/s     (4.8k) | 2.46 GB/s     (2.4k)
Write      | 2.59 GB/s     (5.0k) | 2.63 GB/s     (2.5k)
Total      | 5.05 GB/s     (9.8k) | 5.10 GB/s     (4.9k)
--------------------流媒体解锁--感谢sjlleo开源------------------------
以下测试的解锁地区是准确的，但是不是完整解锁的判断可能有误，这方面仅作参考使用
Youtube
Netflix
[IPv4]
您的出口IP可以使用Netflix，但仅可看Netflix自制剧
NF所识别的IP地域信息：英国
[IPv6]
您的网络可能没有正常配置IPv6，或者没有IPv6网络接入
DisneyPlus
[IPv4]
当前IPv4出口解锁DisneyPlus
区域：英国区
解锁Youtube，Netflix，DisneyPlus上面和下面进行比较，不同之处自行判断
---------------流媒体解锁--感谢RegionRestrictionCheck开源-------------
 以下为IPV4网络测试，若无IPV4网络则无输出
============[ Multination ]============
 Dazn:                                  No
 HotStar:                               Yes (Region: GB)
 Disney+:                               Yes (Region: US)
 Netflix:                               Originals Only
 YouTube Premium:                       Yes (Region: GB)
 Amazon Prime Video:                    Yes (Region: GB)
 TVBAnywhere+:                          Yes
 iQyi Oversea Region:                   GB
 Viu.com:                               No
 YouTube CDN:                           Frankfurt 
 Netflix Preferred CDN:                 Amsterdam  
 Spotify Registration:                  Yes (Region: DE)
 Steam Currency:                        EUR
=======================================
 以下为IPV6网络测试，若无IPV6网络则无输出
----------------TikTok解锁--感谢superbench的开源脚本------------------
 TikTok               : No
-----------------欺诈分数以及IP质量检测--本频道原创-------------------
得分仅作参考，不代表100%准确，IP类型如果不一致请手动查询多个数据库比对
欺诈分数(越低越好)：0
匿名代理: Yes
Tor出口节点: No
服务器IP: No
公共代理: No
网络代理: No
搜索引擎机器人: No
abuse得分： 0
IP2Location数据库IP类型： Data Center/Web Hosting/Transit
ping0数据库IP类型：IDC机房IP
Google搜索可行性：未知
-----------------三网回程--感谢zhanghanyun/backtrace开源--------------
2023/01/08 17:14:56 正在测试三网回程路由...
2023/01/08 17:14:57 北京电信 219.141.136.12  电信163 [普通线路]           
2023/01/08 17:14:57 北京联通 202.106.50.1    联通4837[普通线路]           
2023/01/08 17:14:57 北京移动 221.179.155.161 移动CMI [普通线路]           
2023/01/08 17:14:57 上海电信 202.96.209.133  电信163 [普通线路]           
2023/01/08 17:14:57 上海联通 210.22.97.1     联通4837[普通线路]           
2023/01/08 17:14:57 上海移动 211.136.112.200 移动CMI [普通线路]           
2023/01/08 17:14:57 广州电信 58.60.188.222   电信163 [普通线路]           
2023/01/08 17:14:57 广州联通 210.21.196.6    联通4837[普通线路]           
2023/01/08 17:14:57 广州移动 120.196.165.24  移动CMI [普通线路]           
------------------回程路由--感谢fscarmen开源及PR----------------------
 IPv4 ASN: Twistic Limited
依次测试电信，联通，移动经过的地区及线路，核心程序来由: ipip.net ，请知悉!
广州电信 58.60.188.222
0.09 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
6.08 ms  *  局域网
11.51 ms  AS34927  德国, 黑森州, 法兰克福, ifog.ch
6.79 ms  AS174  德国, 黑森州, 法兰克福, cogentco.com
68.83 ms  AS174  德国, 黑森州, 法兰克福, cogentco.com
305.54 ms  AS4134  中国, 广东, 广州, chinatelecom.com.cn, 电信
314.31 ms  AS134774  中国, 广东, 深圳, chinatelecom.com.cn, 电信
315.59 ms  AS4134  中国, 广东, 深圳, chinatelecom.com.cn, 电信
广州联通 210.21.196.6
0.10 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
5.89 ms  *  局域网
6.42 ms  AS34927  德国, 黑森州, 法兰克福, ifog.ch
12.20 ms  AS34927  荷兰, 北荷兰省, 阿姆斯特丹, ifog.ch
12.11 ms  AS1299  荷兰, 北荷兰省, 阿姆斯特丹, telia.com
12.90 ms  AS1299  荷兰, 北荷兰省, 阿姆斯特丹, telia.com
19.40 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
19.48 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
165.10 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
170.12 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
172.52 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
175.58 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
174.16 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
广州移动 120.196.165.2
0.10 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
5.83 ms  *  局域网
5.78 ms  AS34927  德国, 黑森州, 法兰克福, ifog.ch
11.92 ms  AS34927  荷兰, 北荷兰省, 阿姆斯特丹, ifog.ch
12.76 ms  AS1299  荷兰, 北荷兰省, 阿姆斯特丹, telia.com
13.35 ms  AS1299  荷兰, 北荷兰省, 阿姆斯特丹, telia.com
29.20 ms  AS1299  英国, 伦敦, telia.com
20.37 ms  AS1299  英国, 伦敦, telia.com
24.20 ms  AS1299  英国, 伦敦, telia.com
383.40 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
--------网络测速--由teddysun和superspeed开源及spiritlhls整理----------
测速点位置       上传速度        下载速度        延迟
Speedtest.net    50.38 Mbps      493.25 Mbps     28.54 ms
洛杉矶  　　　   83.79Mbps       31.37Mbps       150.39ms
新加坡  　　　   92.39Mbps       374.97Mbps      213.65ms
中国香港　　�    114.61Mbps      296.53Mbps      197.38ms
电信广东广州5G   0.65Mbps        20.39Mbps       305.21ms
联通上海　　�    44.67Mbps       594.75Mbps      197.27ms
联通湖南长沙�    72.11Mbps       561.38Mbps      167.96ms
移动广西南宁�    4.23Mbps        666.37Mbps      186.87ms
----------------------------------------------------------------------
 总共花费        : 6 分 30 秒
 时间          : Sun Jan  8 17:20:24 HKT 2023
----------------------------------------------------------------------

三网测速：
——————————————————————————————————————————————————————————
ID    测速服务器信息       上传/Mbps   下载/Mbps   延迟/ms
3633  电信|上海　　　　　　↑ 1.11      ↓ 562.53    240.45  
17145 电信|安徽合肥５Ｇ　　↑ 3.80      ↓ 459.30    269.37  
27594 电信|广东广州５Ｇ　　↑ 0.17      ↓ 67.59     266.12  
29353 电信|湖北武汉５Ｇ　　↑ FAILED    ↓ 7.78      278.03  
28225 电信|湖南长沙５Ｇ　　↑ FAILED    ↓ 59.92     249.21  
3973  电信|甘肃兰州　　　　↑ 0.12      ↓ 3.87      193.64  
24447 联通|上海５Ｇ　　　　↑ 162.43    ↓ 478.40    218.01  
4870  联通|湖南长沙　　　　↑ 271.96    ↓ 484.59    184.36  
——————————————————————————————————————————————————————————
  测试完成, 本次测速耗时: 5 分 20 秒
  当前时间: 2023-01-18 16:09:18
```

## 总结

灵车，没钱别碰
