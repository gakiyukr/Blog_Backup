## 前言

OneProvider ，简称 OP~~（原批）~~，知名二道贩子，以转卖别家资源为生。不过倒是老牌商家了，能买到一些奇奇怪怪的机器，比如江苏无锡杜甫、甚至澳门杜甫。~~（就是价格嘛）~~

VPS 可以按时计费，还是不错的，针对于某些临时用途。

## 详细配置

本次测破的是墨西哥最低配，因为某些业务需要墨西哥 IP ，临时开了一台。

```
-------------------- A Bench Script By spiritlhl ---------------------
                   测评频道: https://t.me/vps_reviews                    
版本：2023.05.01
更新日志：融合怪十代目(集合百家之长)(专为测评频道小鸡而生)
-----------------感谢teddysun和superbench和yabs开源-------------------
 CPU 型号          : AMD EPYC Processor
 CPU 核心数        : 1
 CPU 频率          : 3408.000 MHz
 CPU 缓存          : 8192 KB
 硬盘空间          : 9.3 GB (1.2 GB 已用)
 内存              : 473 MB (61 MB 已用)
 Swap              : 510 MB (0 MB 已用)
 系统在线时间      : 0 days, 0 hour 15 min
 负载              : 0.12, 0.11, 0.05
 系统              : Debian GNU/Linux 11 (bullseye)
 AES-NI指令集      : ✔ Enabled
 VM-x/AMD-V支持    : ❌ Disabled
 架构              : x86_64 (64 Bit)
 内核              : 5.10.0-8-amd64
 TCP加速方式       : cubic
 虚拟化架构        : KVM
 ASN组织           : AS136258 BrainStorm Network, Inc
 位置              : Mexico City / MX
 地区              : Mexico City
-------------------CPU测试--感谢lemonbench开源------------------------
 -> CPU 测试中 (Fast Mode, 1-Pass @ 5sec)
 1 线程测试(1核)得分:           738 Scores
-------------------内存测试--感谢lemonbench开源-----------------------
 -> 内存测试 Test (Fast Mode, 1-Pass @ 5sec)
 单线程读测试:          13439.48 MB/s
 单线程写测试:          9455.62 MB/s
----------------磁盘IO读写测试--感谢lemonbench开源--------------------
 -> 磁盘IO测试中 (4K Block/1M Block, Direct Mode)
 测试操作               写速度                                  读速度
 100MB-4K Block         43.3 MB/s (0.09 IOPS, 2.42s))           52.7 MB/s (12872 IOPS, 1.99s)
 1GB-1M Block           1.3 GB/s (1258 IOPS, 0.79s)             2.5 GB/s (2374 IOPS, 0.42s)
-------------------磁盘IO读写测试--感谢yabs开源-----------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 57.02 MB/s   (14.2k) | 75.22 MB/s    (1.1k)
Write      | 57.12 MB/s   (14.2k) | 75.62 MB/s    (1.1k)
Total      | 114.14 MB/s  (28.5k) | 150.84 MB/s   (2.3k)           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 78.60 MB/s     (153) | 74.38 MB/s      (72)
Write      | 82.77 MB/s     (161) | 79.33 MB/s      (77)
Total      | 161.38 MB/s    (314) | 153.71 MB/s    (149)
--------------------流媒体解锁--感谢sjlleo开源------------------------
以下测试的解锁地区是准确的，但是不是完整解锁的判断可能有误，这方面仅作参考使用
----------------Youtube----------------
[IPv4]
连接方式: Google Global CacheCDN (ISP Cooperation)
ISP运营商: TRANSTELCO
视频缓存节点地域: 墨西哥墨西哥城(MEX3)
Youtube识别地域: 墨西哥(MX)
----------------Netflix----------------
[IPv4]
您的出口IP可以使用Netflix，但仅可看Netflix自制剧
NF所识别的IP地域信息：墨西哥
[IPv6]
您的网络可能没有正常配置IPv6，或者没有IPv6网络接入
---------------DisneyPlus---------------
[IPv4]
当前IPv4出口解锁DisneyPlus
区域：墨西哥区
解锁Youtube，Netflix，DisneyPlus上面和下面进行比较，不同之处自行判断
---------------流媒体解锁--感谢RegionRestrictionCheck开源-------------
 以下为IPV4网络测试，若无IPV4网络则无输出
============[ Multination ]============
 Dazn:                                  No
 HotStar:                               No
 Disney+:                               No
 Netflix:                               Originals Only
 YouTube Premium:                       Yes (Region: MX)
 Amazon Prime Video:                    Yes (Region: MX)
 TVBAnywhere+:                          Yes
 iQyi Oversea Region:                   MX
 Viu.com:                               No
 YouTube CDN:                           Associated with [TRANSTELCO]
 Netflix Preferred CDN:                 Associated with [Transtelco] in [Mexico City ]
 Spotify Registration:                  No
 Steam Currency:                        MXN
=======================================
 以下为IPV6网络测试，若无IPV6网络则无输出
-------------TikTok解锁--感谢lmc999的源脚本及fscarmen PR--------------
 Tiktok Region:         【MX】
--------OpenAi解锁--感谢missuo的OpenAI-Checker项目本人修改优化--------
[IPv4]
Your IP supports access to OpenAI. Region: MX
[IPv6]
IPv6 is not supported on the current host. Skip...
-----------------欺诈分数以及IP质量检测--本频道原创-------------------
以下仅作参考，不代表100%准确，如果和实际情况不一致请手动查询多个数据库比对
scamalytics数据库:
  欺诈分数(越低越好)：83
  匿名代理: No
  Tor出口节点: No
  服务器IP: Yes
  公共代理: No
  网络代理: No
  搜索引擎机器人: No
ip234数据库：
  欺诈分数(越低越好)：1
ip-api数据库:
  手机流量: No
  代理服务: No
  数据中心: Yes
abuseipdb数据库-abuse得分：0
IP类型:
  IP2Location数据库: Data Center/Web Hosting/Transit
Google搜索可行性：YES
-----------------三网回程--感谢zhanghanyun/backtrace开源--------------
2023/05/01 22:41:12 北京电信 219.141.136.12  电信163 [普通线路]           
2023/05/01 22:41:12 北京联通 202.106.50.1    联通4837[普通线路]           
2023/05/01 22:41:12 北京移动 221.179.155.161 移动CMI [普通线路]           
2023/05/01 22:41:12 上海电信 202.96.209.133  电信163 [普通线路]           
2023/05/01 22:41:12 上海联通 210.22.97.1     联通4837[普通线路]           
2023/05/01 22:41:12 上海移动 211.136.112.200 移动CMI [普通线路]           
2023/05/01 22:41:12 广州电信 58.60.188.222   电信163 [普通线路]           
2023/05/01 22:41:12 广州联通 210.21.196.6    联通4837[普通线路]           
2023/05/01 22:41:12 广州移动 120.196.165.24  移动CMI [普通线路]           
2023/05/01 22:41:12 成都电信 61.139.2.69     电信163 [普通线路]           
2023/05/01 22:41:12 成都联通 119.6.6.6       联通4837[普通线路]           
2023/05/01 22:41:12 成都移动 211.137.96.205  移动CMI [普通线路]           
------------------回程路由--感谢fscarmen开源及PR----------------------
IPv4 ASN: BrainStorm Network
依次测试电信，联通，移动经过的地区及线路，核心程序来由: ipip.net ，请知悉!
广州电信 58.60.188.222
33.76 ms  AS396356  墨西哥, 墨西哥联邦区, 墨西哥城, mytrinity.com.ua
1.22 ms  AS174  墨西哥, 墨西哥联邦区, 墨西哥城, cogentco.com
14.15 ms  AS174  美国, 德克萨斯州, 麦卡伦, cogentco.com
30.67 ms  AS174  美国, 德克萨斯州, 休斯顿, cogentco.com
46.73 ms  AS174  美国, 德克萨斯州, 埃尔帕索, cogentco.com
52.73 ms  AS174  美国, 亚利桑那州, 凤凰城, cogentco.com
68.63 ms  AS174  美国, 加利福尼亚州, 洛杉矶, cogentco.com
73.11 ms  AS174  美国, 加利福尼亚州, 圣何塞, cogentco.com
73.19 ms  AS174  美国, 加利福尼亚州, 圣何塞, cogentco.com
71.61 ms  AS174  美国, 加利福尼亚州, 圣何塞, cogentco.com
215.23 ms  AS4134  中国, 广东, 深圳, chinatelecom.com.cn, 电信
222.87 ms  AS4134  中国, 广东, 深圳, chinatelecom.com.cn, 电信
广州联通 210.21.196.6
0.50 ms  AS396356  墨西哥, 墨西哥联邦区, 墨西哥城, mytrinity.com.ua
0.27 ms  AS32098  墨西哥, transtelco.net
1.03 ms  AS32098  墨西哥, 墨西哥联邦区, 墨西哥城, transtelco.net
1.09 ms  AS32098  墨西哥, transtelco.net
32.45 ms  AS32098  美国, 德克萨斯州, 达拉斯, transtelco.net
32.88 ms  AS6453  美国, 德克萨斯州, 达拉斯, tatacommunications.com
68.18 ms  AS6453  美国, 加利福尼亚州, 洛杉矶, tatacommunications.com
257.75 ms  AS4837  美国, 加利福尼亚州, 洛杉矶, chinaunicom.com, 联通
225.65 ms  AS4837  中国, 北京, chinaunicom.com, 联通
264.67 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
299.90 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
287.77 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
309.69 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
288.75 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
广州移动 120.196.165.2
0.26 ms  AS396356  墨西哥, 墨西哥联邦区, 墨西哥城, mytrinity.com.ua
1.22 ms  AS174  墨西哥, 墨西哥联邦区, 墨西哥城, cogentco.com
14.05 ms  AS174  美国, 德克萨斯州, 麦卡伦, cogentco.com
27.72 ms  AS174  美国, 德克萨斯州, 休斯顿, cogentco.com
46.36 ms  AS174  美国, 德克萨斯州, 埃尔帕索, cogentco.com
51.50 ms  AS174  美国, 亚利桑那州, 凤凰城, cogentco.com
66.05 ms  AS174  美国, 加利福尼亚州, 洛杉矶, cogentco.com
66.30 ms  AS174  美国, 加利福尼亚州, 洛杉矶, cogentco.com
64.44 ms  AS174  美国, 加利福尼亚州, 洛杉矶, cogentco.com
64.78 ms  AS58453  美国, 加利福尼亚州, 洛杉矶, chinamobile.com, 移动
63.42 ms  AS58453  美国, 加利福尼亚州, 洛杉矶, chinamobile.com, 移动
244.25 ms  AS9808  中国, 上海, chinamobile.com, 移动
248.14 ms  AS9808  中国, 上海, chinamobile.com, 移动
273.35 ms  AS56040  中国, 广东, 广州, chinamobile.com, 移动
281.68 ms  AS56040  中国, 广东, 深圳, chinamobile.com, 移动
------------------------ ecs-net--本频道独创 -------------------------
位置             上传速度        下载速度        延迟     丢包率
Speedtest.net    3197.78 Mbps    2194.04 Mbps    1.87     NULL
洛杉矶           1025.90 Mbps    1020.24 Mbps    60.84    0.0%
新加坡           208.63 Mbps     445.46 Mbps     259.49   0.0%
联通沈阳         4.82 Mbps       29.37 Mbps      271.85   8.4%
联通WuXi         314.95 Mbps     395.47 Mbps     269.21   0.0%
电信Suzhou5G     360.77 Mbps     700.94 Mbps     197.07   NULL
电信湖南5G       0.88 Mbps       48.98 Mbps      231.18   4.6%
移动Chengdu      246.87 Mbps     352.62 Mbps     267.57   0.0%
----------------------------------------------------------------------
 总共花费      : 9 分 50 秒
 时间          : Mon May  1 22:46:37 EDT 2023
----------------------------------------------------------------------
ID    测速服务器信息       上传/Mbps   下载/Mbps   延迟/ms
3633  电信|上海　　　　　　↑ 278.38    ↓ 609.57    210.83  
17145 电信|安徽合肥５Ｇ　　↑ 212.45    ↓ 439.36    206.16  
27594 电信|广东广州５Ｇ　　↑ 3.26      ↓ 17.44     225.19  
5396  电信|江苏苏州５Ｇ　　↑ 211.04    ↓ 954.52    192.58  
23844 电信|湖北武汉　　　　↑ 2.64      ↓ 514.40    226.69  
28225 电信|湖南长沙５Ｇ　　↑ 0.90      ↓ 25.95     222.65  
3973  电信|甘肃兰州　　　　↑ 10.55     ↓ 105.84    232.61  
24447 联通|上海５Ｇ　　　　↑ 6.97      ↓ 498.59    271.67  
4870  联通|湖南长沙　　　　↑ 243.74    ↓ 98.36     262.60  
25858 移动|北京　　　　　　↑ 0.26      ↓ 148.34    521.79  
----------------------------------------------------------------------
[Info] 测试路由 到 上海电信(天翼云) 中 ...
traceroute to 101.227.255.45 (101.227.255.45), 30 hops max, 32 byte packets
 1  5-105-231-2.flemservices.com (5.105.231.2)  0.45 ms  AS396356  Mexico, The Federal District of Mexico, Mexico City, mytrinity.com.ua
 2  *
 3  154.24.81.141  1.02 ms  AS174  Mexico, The Federal District of Mexico, Mexico City, cogentco.com
 4  be2636.ccr21.mfe02.atlas.cogentco.com (154.54.85.181)  14.00 ms  AS174  United States, Texas, McAllen, cogentco.com
 5  be2887.ccr41.iah01.atlas.cogentco.com (154.54.47.33)  27.77 ms  AS174  United States, Texas, Houston, cogentco.com
 6  be3850.ccr21.elp02.atlas.cogentco.com (154.54.0.54)  46.46 ms  AS174  United States, Texas, El Paso, cogentco.com
 7  be2979.ccr31.phx01.atlas.cogentco.com (154.54.5.217)  51.52 ms  AS174  United States, Arizona, Phoenix, cogentco.com
 8  be2931.ccr41.lax01.atlas.cogentco.com (154.54.44.86)  66.08 ms  AS174  United States, California, Los Angeles, cogentco.com
 9  be3176.ccr21.sjc01.atlas.cogentco.com (154.54.31.190)  73.27 ms  AS174  United States, California, San Jose, cogentco.com
10  be3142.ccr41.sjc03.atlas.cogentco.com (154.54.1.194)  74.22 ms  AS174  United States, California, San Jose, cogentco.com
11  38.104.138.106  68.71 ms  AS174  United States, California, San Jose, cogentco.com
12  *
13  202.97.33.125  239.71 ms  AS4134  China, Shanghai, ChinaTelecom
14  *
15  *
16  124.74.166.222  207.65 ms  AS4812  China, Shanghai, ChinaTelecom
17  *
18  *
19  *
20  *
21  *
22  *
23  *
24  *
25  *
26  *
27  *
28  *
29  *
30  *

[Info] 测试路由 到 上海电信(天翼云) 完成 ！
[Info] 测试路由 到 厦门电信CN2 中 ...
traceroute to 117.28.254.129 (117.28.254.129), 30 hops max, 32 byte packets
 1  5-105-231-2.flemservices.com (5.105.231.2)  0.31 ms  AS396356  Mexico, The Federal District of Mexico, Mexico City, mytrinity.com.ua
 2  *
 3  154.24.81.141  1.28 ms  AS174  Mexico, The Federal District of Mexico, Mexico City, cogentco.com
 4  be2636.ccr21.mfe02.atlas.cogentco.com (154.54.85.181)  13.94 ms  AS174  United States, Texas, McAllen, cogentco.com
 5  be2887.ccr41.iah01.atlas.cogentco.com (154.54.47.33)  28.36 ms  AS174  United States, Texas, Houston, cogentco.com
 6  be3850.ccr21.elp02.atlas.cogentco.com (154.54.0.54)  46.18 ms  AS174  United States, Texas, El Paso, cogentco.com
 7  be2979.ccr31.phx01.atlas.cogentco.com (154.54.5.217)  52.71 ms  AS174  United States, Arizona, Phoenix, cogentco.com
 8  be2931.ccr41.lax01.atlas.cogentco.com (154.54.44.86)  67.75 ms  AS174  United States, California, Los Angeles, cogentco.com
 9  be2327.ccr21.hkg02.atlas.cogentco.com (154.54.0.6)  211.75 ms  AS174  China, Hong Kong, cogentco.com
10  hgc.demarc.cogentco.com (154.18.4.226)  206.41 ms  AS174  China, Hong Kong, cogentco.com
11  218.188.104.218  206.66 ms  AS9304  China, Hong Kong, hgc.com.hk
12  59.43.183.109  218.25 ms  *  China, Guangdong, Guangzhou, ChinaTelecom
13  *
14  *
15  59.43.46.214  242.46 ms  *  China, Fujian, Fuzhou, ChinaTelecom
16  *
17  *
18  *
19  *
20  117.28.254.129  253.43 ms  AS4809  China, Fujian, Xiamen, ChinaTelecom

[Info] 测试路由 到 厦门电信CN2 完成 ！
[Info] 测试路由 到 浙江杭州联通 中 ...
traceroute to 101.71.241.238 (101.71.241.238), 30 hops max, 32 byte packets
 1  5-105-231-2.flemservices.com (5.105.231.2)  0.53 ms  AS396356  Mexico, The Federal District of Mexico, Mexico City, mytrinity.com.ua
 2  *
 3  201-174-254-180.transtelco.net (201.174.254.180)  1.03 ms  AS32098  Mexico, The Federal District of Mexico, Mexico City, transtelco.net
 4  201-174-251-225.transtelco.net (201.174.251.225)  1.10 ms  AS32098  Mexico, transtelco.net
 5  201-174-255-85.transtelco.net (201.174.255.85)  32.50 ms  AS32098  United States, Texas, Dallas, transtelco.net
 6  201-174-254-39.transtelco.net (201.174.254.39)  29.63 ms  AS32098  United States, Texas, Dallas, transtelco.net
 7  ae7.cr7-dal3.ip4.gtt.net (208.116.218.89)  33.92 ms  AS3257  United States, Texas, Dallas, gtt.net
 8  ae27.cr2-sjc1.ip4.gtt.net (89.149.141.29)  69.51 ms  AS3257  United States, California, San Jose, gtt.net
 9  as4837.cr5-sjc1.ip4.gtt.net (173.205.56.206)  326.89 ms  AS3257  United States, California, San Jose, gtt.net
10  219.158.97.177  350.51 ms  AS4837  China, Shanghai, ChinaUnicom
11  219.158.113.126  352.53 ms  AS4837  China, Shanghai, ChinaUnicom
12  219.158.113.101  353.55 ms  AS4837  China, Shanghai, ChinaUnicom
13  *
14  101.69.245.206  384.35 ms  AS4837  China, Zhejiang, Hangzhou, ChinaUnicom
15  *
16  *
17  *
18  *
19  *
20  *
21  *
22  *
23  *
24  *
25  *
26  *
27  *
28  *
29  *
30  *

[Info] 测试路由 到 浙江杭州联通 完成 ！
[Info] 测试路由 到 浙江杭州移动 中 ...
traceroute to 112.17.0.106 (112.17.0.106), 30 hops max, 32 byte packets
 1  5-105-231-2.flemservices.com (5.105.231.2)  0.42 ms  AS396356  Mexico, The Federal District of Mexico, Mexico City, mytrinity.com.ua
 2  *
 3  154.24.81.141  1.20 ms  AS174  Mexico, The Federal District of Mexico, Mexico City, cogentco.com
 4  be2636.ccr21.mfe02.atlas.cogentco.com (154.54.85.181)  14.31 ms  AS174  United States, Texas, McAllen, cogentco.com
 5  be2887.ccr41.iah01.atlas.cogentco.com (154.54.47.33)  28.54 ms  AS174  United States, Texas, Houston, cogentco.com
 6  be3850.ccr21.elp02.atlas.cogentco.com (154.54.0.54)  46.11 ms  AS174  United States, Texas, El Paso, cogentco.com
 7  be2979.ccr31.phx01.atlas.cogentco.com (154.54.5.217)  52.89 ms  AS174  United States, Arizona, Phoenix, cogentco.com
 8  be2931.ccr41.lax01.atlas.cogentco.com (154.54.44.86)  66.14 ms  AS174  United States, California, Los Angeles, cogentco.com
 9  be3243.ccr41.lax05.atlas.cogentco.com (154.54.27.118)  66.35 ms  AS174  United States, California, Los Angeles, cogentco.com
10  *
11  *
12  223.120.12.178  533.72 ms  AS58453  China, Shanghai, ChinaMobile
13  *
14  221.183.89.33  550.17 ms  AS9808  China, Shanghai, ChinaMobile
15  221.183.89.30  567.16 ms  AS9808  China, Zhejiang, Hangzhou, ChinaMobile
16  *
17  *
18  *
19  *
20  *
21  *
22  *
23  *
24  *
25  *
26  *
27  *
28  *
29  *
30  *

[Info] 测试路由 到 浙江杭州移动 完成 ！
[Info] 测试路由 到 北京教育网 中 ...
traceroute to 202.205.6.30 (202.205.6.30), 30 hops max, 32 byte packets
 1  5-105-231-2.flemservices.com (5.105.231.2)  0.41 ms  AS396356  Mexico, The Federal District of Mexico, Mexico City, mytrinity.com.ua
 2  *
 3  154.24.81.141  2.06 ms  AS174  Mexico, The Federal District of Mexico, Mexico City, cogentco.com
 4  be2637.ccr22.mfe02.atlas.cogentco.com (154.54.85.185)  13.88 ms  AS174  United States, Texas, McAllen, cogentco.com
 5  be2888.ccr42.iah01.atlas.cogentco.com (154.54.47.45)  27.12 ms  AS174  United States, Texas, Houston, cogentco.com
 6  be3851.ccr22.elp02.atlas.cogentco.com (154.54.2.6)  43.65 ms  AS174  United States, Texas, El Paso, cogentco.com
 7  be3872.ccr32.phx01.atlas.cogentco.com (154.54.26.53)  54.52 ms  AS174  United States, Arizona, Phoenix, cogentco.com
 8  be2932.ccr42.lax01.atlas.cogentco.com (154.54.45.162)  64.08 ms  AS174  United States, California, Los Angeles, cogentco.com
 9  be3360.ccr41.lax04.atlas.cogentco.com (154.54.25.150)  63.21 ms  AS174  United States, California, Los Angeles, cogentco.com
10  38.88.196.186  66.57 ms  AS174  United States, California, Los Angeles, cogentco.com
11  101.4.117.169  208.07 ms  AS4538  China, Beijing, CHINAEDU
12  *
13  101.4.118.213  209.92 ms  AS4538  China, Beijing, CHINAEDU
14  *
15  219.224.102.230  212.18 ms  AS4538  China, Beijing, CHINAEDU
16  *
17  *
18  *
19  *
20  *
21  *
22  *
23  *
24  *
25  *
26  *
27  *
28  *
29  *
30  *

[Info] 测试路由 到 北京教育网 完成 ！
[Info] 四网路由快速测试 已完成 ！
----------------------------------------------------------------------
```

![](https://www.speedtest.net/result/c/906ada6f-4c72-4a97-8733-cc2ee58d1cd9.png)