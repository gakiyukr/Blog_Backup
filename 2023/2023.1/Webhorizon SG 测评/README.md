官网上好像没找的这个的配置，好像是绝版了？找MJJ 15收来的

虽然产品页上写的1胖子/月，但是实际下单的时候，每月会额外收0.4胖子的IP费用，所以每月实际是1.4胖子/月。

小鸡是LXC架构，而不是KVM~~（这价格还要什么自行车，买他不就是为了流媒体吗）~~

![](https://s3-jp-ap-3.040407.xyz/oss/photos/5934855281165053859_121.jpg)

## 性能测试

```
-------------------- A Bench Script By spiritlhl ---------------------
                   测评频道: https://t.me/vps_reviews                    
版本：2023.01.20
更新日志：融合怪九代目(集合百家之长)(专为测评频道小鸡而生)
-----------------感谢teddysun和superbench和yabs开源-------------------
 CPU 型号          : AMD EPYC 7502P 32-Core Processor
 CPU 核心数        : 1
 CPU 频率          : 2500.000 MHz
 CPU 缓存          : 512 KB
 硬盘空间          : 10.0 GB (0.5 GB 已用)
 内存              : 512 MB (41 MB 已用)
 Swap              : 0 MB (0 MB 已用)
 系统在线时间      : 0 days, 0 hour 10 min
 负载              : 0.22, 0.16, 0.07
 系统              : Debian GNU/Linux 11 (bullseye)
 AES-NI指令集      : ✔ Enabled
 VM-x/AMD-V支持    : ✔ Enabled
 架构              : x86_64 (64 Bit)
 内核              : 5.15.74-1-pve
 TCP加速方式       : bbr
 虚拟化架构        : LXC
 ASN组织           : AS149020 WebHorizon Internet Services
 位置              : Singapore / SG
 地区              : Singapore
-------------------CPU测试--感谢lemonbench开源------------------------
 -> CPU 测试中 (Fast Mode, 1-Pass @ 5sec)
 1 线程测试(1核)得分:           1653 Scores
-------------------内存测试--感谢lemonbench开源-----------------------
 -> 内存测试 Test (Fast Mode, 1-Pass @ 5sec)
 单线程读测试:          44003.16 MB/s
 单线程写测试:          18803.01 MB/s
----------------磁盘IO读写测试--感谢lemonbench开源--------------------
 -> 磁盘IO测试中 (4K Block/1M Block, Direct Mode)
 测试操作               写速度                                  读速度
 100MB-4K Block         910 MB/s (0.00 IOPS, 0.12s))            570 MB/s (139260 IOPS, 0.18s)
 1GB-1M Block           2.0 GB/s (1879 IOPS, 0.53s)             6.7 GB/s (6429 IOPS, 0.16s)
-------------------磁盘IO读写测试--感谢yabs开源-----------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 5.73 MB/s     (1.4k) | 92.29 MB/s    (1.4k)
Write      | 5.71 MB/s     (1.4k) | 92.78 MB/s    (1.4k)
Total      | 11.45 MB/s    (2.8k) | 185.08 MB/s   (2.8k)           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 182.93 MB/s    (357) | 221.54 MB/s    (216)
Write      | 192.65 MB/s    (376) | 236.29 MB/s    (230)
Total      | 375.59 MB/s    (733) | 457.84 MB/s    (446)
--------------------流媒体解锁--感谢sjlleo开源------------------------
以下测试的解锁地区是准确的，但是不是完整解锁的判断可能有误，这方面仅作参考使用
Youtube
[IPv4]
连接方式: Youtube Video Server
视频缓存节点地域: 新加坡 新加坡/樟宜  (SIN10S14)
Youtube识别地域: 新加坡(SG)

[IPv6]
连接方式: Youtube Video Server
视频缓存节点地域: 新加坡 新加坡/樟宜  (SIN10S14)
Youtube识别地域: 无信息(null)
Netflix
[IPv4]
您的出口IP完整解锁Netflix，支持非自制剧的观看
NF所识别的IP地域信息：新加坡
[IPv6]
您的出口IP完整解锁Netflix，支持非自制剧的观看
NF所识别的IP地域信息：新加坡
DisneyPlus
[IPv4]
当前IPv4出口解锁DisneyPlus
区域：新加坡区

[IPv6]
当前IPv6出口解锁DisneyPlus
区域：新加坡区
解锁Youtube，Netflix，DisneyPlus上面和下面进行比较，不同之处自行判断
---------------流媒体解锁--感谢RegionRestrictionCheck开源-------------
 以下为IPV4网络测试，若无IPV4网络则无输出
============[ Multination ]============
 Dazn:                                  No
 HotStar:                               No
 Disney+:                               Yes (Region: SG)
 Netflix:                               Yes (Region: SG)
 YouTube Premium:                       Yes (Region: SG)
 Amazon Prime Video:                    Yes (Region: SG)
 TVBAnywhere+:                          Yes
 iQyi Oversea Region:                   JP
 Viu.com:                               No
 YouTube CDN:                           Singapore 
 Netflix Preferred CDN:                 Singapore  
 Spotify Registration:                  No
 Steam Currency:                        SGD
=======================================
 以下为IPV6网络测试，若无IPV6网络则无输出
============[ Multination ]============
 Dazn:                                  Failed (Network Connection)
 HotStar:                               Yes (Region: SG)
 Disney+:                               Yes (Region: SG)
 Netflix:                               Yes (Region: SG)
 YouTube Premium:                       No  (Region: CN) 
 Amazon Prime Video:                    Unsupported
 TVBAnywhere+:                          Failed (Network Connection)
 iQyi Oversea Region:                   Failed
 Viu.com:                               Failed
 YouTube CDN:                           Singapore 
 Netflix Preferred CDN:                 Singapore  
 Spotify Registration:                  No
 Steam Currency:                        Failed (Network Connection)
=======================================
-------------TikTok解锁--感谢lmc999加密脚本及fscarmen PR--------------
 Tiktok Region:         【JP】
-----------------欺诈分数以及IP质量检测--本频道原创-------------------
以下仅作参考，不代表100%准确，如果和实际情况不一致请手动查询多个数据库比对
欺诈分数(越低越好)：0
匿名代理: No
Tor出口节点: No
服务器IP: Yes
公共代理: No
网络代理: No
搜索引擎机器人: No
abuse得分： 0
IP2Location数据库IP类型： Data Center/Web Hosting/Transit
ping0数据库IP类型：IDC机房IP
Google搜索可行性：未知
-----------------三网回程--感谢zhanghanyun/backtrace开源--------------
2023/01/21 00:42:27 北京电信 219.141.136.12  测试超时
2023/01/21 00:42:27 北京联通 202.106.50.1    联通4837[普通线路]           
2023/01/21 00:42:27 北京移动 221.179.155.161 移动CMI [普通线路]           
2023/01/21 00:42:27 上海电信 202.96.209.133  电信163 [普通线路]           
2023/01/21 00:42:27 上海联通 210.22.97.1     联通4837[普通线路]           
2023/01/21 00:42:27 上海移动 211.136.112.200 移动CMI [普通线路]           
2023/01/21 00:42:27 广州电信 58.60.188.222   电信163 [普通线路]           
2023/01/21 00:42:27 广州联通 210.21.196.6    联通4837[普通线路]           
2023/01/21 00:42:27 广州移动 120.196.165.24  移动CMI [普通线路]           
2023/01/21 00:42:27 成都电信 61.139.2.69     电信163 [普通线路]           
2023/01/21 00:42:27 成都联通 119.6.6.6       联通4837[普通线路]           
2023/01/21 00:42:27 成都移动 211.137.96.205  移动CMI [普通线路]           
------------------回程路由--感谢fscarmen开源及PR----------------------
IPv4 ASN: WebHorizon Internet Services
IPv6 ASN: WebHorizon Internet Services
依次测试电信，联通，移动经过的地区及线路，核心程序来由: ipip.net ，请知悉!
广州电信 58.60.188.222
0.22 ms  AS136557  新加坡, hostuniversal.com.au
1.28 ms  AS174  新加坡, cogentco.com
1.59 ms  AS174  新加坡, cogentco.com
1.92 ms  AS174  新加坡, cogentco.com
225.02 ms  AS174  澳大利亚, 西澳大利亚州, 珀斯, cogentco.com
225.28 ms  AS174  澳大利亚, 新南威尔士州, 悉尼, cogentco.com
225.13 ms  AS174  美国, 加利福尼亚州, 洛杉矶, cogentco.com
225.36 ms  AS174  美国, 加利福尼亚州, 洛杉矶, cogentco.com
225.44 ms  AS174  美国, 加利福尼亚州, 洛杉矶, cogentco.com
238.13 ms  AS174  美国, 加利福尼亚州, 圣何塞, cogentco.com
263.38 ms  AS174  美国, 加利福尼亚州, 圣何塞, cogentco.com
264.54 ms  AS174  美国, 加利福尼亚州, 圣何塞, cogentco.com
408.47 ms  AS4134  中国, 广东, 广州, chinatelecom.com.cn, 电信
390.21 ms  AS4134  中国, 广东, 广州, chinatelecom.com.cn, 电信
411.25 ms  AS4134  中国, 广东, 广州, chinatelecom.com.cn, 电信
387.68 ms  AS134774  中国, 广东, 深圳, chinatelecom.com.cn, 电信
390.80 ms  AS4134  中国, 广东, 深圳, chinatelecom.com.cn, 电信
广州联通 210.21.196.6
0.20 ms  AS136557  新加坡, hostuniversal.com.au
1.13 ms  AS174  新加坡, cogentco.com
1.38 ms  AS174  新加坡, cogentco.com
1.51 ms  AS174  新加坡, cogentco.com
224.75 ms  AS174  澳大利亚, 西澳大利亚州, 珀斯, cogentco.com
225.10 ms  AS174  澳大利亚, 新南威尔士州, 悉尼, cogentco.com
224.84 ms  AS174  美国, 加利福尼亚州, 洛杉矶, cogentco.com
225.25 ms  AS174  美国, 加利福尼亚州, 洛杉矶, cogentco.com
225.69 ms  AS174  美国, 加利福尼亚州, 洛杉矶, cogentco.com
235.42 ms  AS174  美国, 加利福尼亚州, 洛杉矶, cogentco.com
253.16 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
249.94 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
250.14 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
254.23 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
254.90 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
广州移动 120.196.165.2
0.21 ms  AS136557  新加坡, hostuniversal.com.au
0.97 ms  AS136557  新加坡, hostuniversal.com.au
0.99 ms  AS60068  欧洲地区, datacamp.co.uk
1.82 ms  AS2914  新加坡, ntt.com
41.65 ms  AS2914  中国, 香港, ntt.com
38.79 ms  AS2914  中国, 香港, ntt.com
42.78 ms  AS58453  中国, 广东, 广州, chinamobile.com, 移动
42.89 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
45.10 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
44.02 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
45.17 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
49.71 ms  AS9808  中国, 广东, 深圳, chinamobile.com, 移动
52.03 ms  AS56040  中国, 广东, 深圳, chinamobile.com, 移动
--------网络测速--由teddysun和superspeed开源及spiritlhls整理----------
测速点位置       上传速度        下载速度        延迟
Speedtest.net    866.60 Mbps     903.82 Mbps     67.38 ms
洛杉矶           423.13 Mbps     904.59 Mbps     180.04 ms
新加坡           932.46 Mbps     905.37 Mbps     2.02 ms
中国香港         913.22 Mbps     922.69 Mbps     30.80 ms
电信上海         155.39 Mbps     819.40 Mbps     332.01 ms
电信广东广州5G   175.55 Mbps     124.07 Mbps     406.33 ms
联通上海         204.05 Mbps     827.51 Mbps     352.28 ms
联通湖南长沙     896.03 Mbps     16.42 Mbps      44.67 ms
移动广西南宁     324.78 Mbps     834.06 Mbps     228.57 ms
----------------------------------------------------------------------
 总共花费      : 8 分 23 秒
 时间          : Sat Jan 21 00:47:53 UTC 2023
----------------------------------------------------------------------
```

## 流媒体测试

这才是本文的大头

```
============[ Multination ]============
 Dazn:                                  No
 HotStar:                               No
 Disney+:                               Yes (Region: SG)
 Netflix:                               Yes (Region: SG)
 YouTube Premium:                       Yes (Region: SG)
 Amazon Prime Video:                    Yes (Region: SG)
 TVBAnywhere+:                          Yes
 iQyi Oversea Region:                   JP
 Viu.com:                               Yes (Region: SG)
 YouTube CDN:                           Singapore 
 Netflix Preferred CDN:                 Singapore  
 Spotify Registration:                  No
 Steam Currency:                        SGD
=======================================
=============[ Hong Kong ]=============
 Now E:                                 No
 Viu.TV:                                No
 MyTVSuper:                             No
 HBO GO Asia:                           Yes (Region: SG)
 BiliBili Hongkong/Macau/Taiwan:        No
=======================================
===============[ Japan ]===============
 DMM:                                   Yes
 DMM TV:                                No
 Abema.TV:                              No
 Niconico:                              No
 music.jp:                              No
 Telasa:                                Yes
 Paravi:                                No
 U-NEXT:                                No
 Hulu Japan:                            Yes
 TVer:                                  Yes
 GYAO!:                                 No
 WOWOW:                                 Failed
 VideoMarket:                           Yes
 FOD(Fuji TV):                          No
 Radiko:                                No
 Karaoke@DAM:                           No
 J:com On Demand:                       No
 ---Game---
 Kancolle Japan:                        Yes
 Pretty Derby Japan:                    Yes
 Konosuba Fantastic Days:               Yes
 Princess Connect Re:Dive Japan:        Yes
 World Flipper Japan:                   Yes
 Project Sekai: Colorful Stage:         Yes
=======================================
==============[ Oceania ]==============
 NBA TV:                                Yes
 Acorn TV:                              Yes
 SHOWTIME:                              Yes
 BritBox:                               Yes
 Funimation:                            No
 Paramount+:                            No
 =======================================
```

流媒体还是不错的（日本游戏解锁没想到）

## 总结

买来看流媒体还行，200G流量足够日常轻量使用，毕竟价钱在这摆着，要求不能太高。

山东移动直连，速度还不错，能跑满我的百兆小水管

![](https://www.speedtest.net/result/14238007645.png)