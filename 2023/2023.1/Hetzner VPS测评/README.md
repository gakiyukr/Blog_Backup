Hetzner（一般简称HZ）与OVH，Netcup统称欧洲三大金刚。HZ的免税或者是验证倒是没那么严，PayPal预充值20 EUR就行，相比OVH歧视国人、NC要企业身份还是很友好的。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_01-22_22-43-07.png)

价格方面个人建站CX11 CXP11都可以，根据自己网站的流量选择。个人不建议选德国机房，HZ德国知名的盒子战车，邻居全是刷PT的~~（说不定是内网互刷）~~。不过其他机房刷PT也不错~~（问就是用过芬兰机房刷PT）~~

本次测评测试CX11的德国机房（流媒体啥的就算了吧）

## 性能测试

```
-------------------- A Bench Script By spiritlhl ---------------------
                   测评频道: https://t.me/vps_reviews                    
版本：2023.01.20
更新日志：融合怪九代目(集合百家之长)(专为测评频道小鸡而生)
-----------------感谢teddysun和superbench和yabs开源-------------------
 CPU 型号          : Intel Xeon Processor (Skylake, IBRS)
 CPU 核心数        : 1
 CPU 频率          : 2294.608 MHz
 CPU 缓存          : 16384 KB
 硬盘空间          : 19.1 GB (1.4 GB 已用)
 内存              : 1935 MB (66 MB 已用)
 Swap              : 0 MB (0 MB 已用)
 系统在线时间      : 0 days, 0 hour 3 min
 负载              : 0.14, 0.06, 0.01
 系统              : Debian GNU/Linux 11 (bullseye)
 AES-NI指令集      : ✔ Enabled
 VM-x/AMD-V支持    : ❌ Disabled
 架构              : x86_64 (64 Bit)
 内核              : 5.10.0-19-amd64
 TCP加速方式       : cubic
 虚拟化架构        : KVM
 ASN组织           : AS24940 Hetzner Online GmbH
 位置              : Gunzenhausen / DE
 地区              : Bavaria
-------------------CPU测试--感谢lemonbench开源------------------------
 -> CPU 测试中 (Fast Mode, 1-Pass @ 5sec)
 1 线程测试(1核)得分:           903 Scores
-------------------内存测试--感谢lemonbench开源-----------------------
 -> 内存测试 Test (Fast Mode, 1-Pass @ 5sec)
 单线程读测试:          17826.69 MB/s
 单线程写测试:          12880.49 MB/s
----------------磁盘IO读写测试--感谢lemonbench开源--------------------
 -> 磁盘IO测试中 (4K Block/1M Block, Direct Mode)
 测试操作               写速度                                  读速度
 100MB-4K Block         32.2 MB/s (7868 IOPS, 3.25s)            51.4 MB/s (12553 IOPS, 2.04s)
 1GB-1M Block           773 MB/s (737 IOPS, 1.36s)              1.1 GB/s (1052 IOPS, 0.95s)
-------------------磁盘IO读写测试--感谢yabs开源-----------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 123.73 MB/s  (30.9k) | 1.41 GB/s    (22.0k)
Write      | 124.05 MB/s  (31.0k) | 1.42 GB/s    (22.1k)
Total      | 247.78 MB/s  (61.9k) | 2.83 GB/s    (44.2k)           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 2.58 GB/s     (5.0k) | 3.02 GB/s     (2.9k)
Write      | 2.72 GB/s     (5.3k) | 3.22 GB/s     (3.1k)
Total      | 5.31 GB/s    (10.3k) | 6.25 GB/s     (6.1k)
--------------------流媒体解锁--感谢sjlleo开源------------------------
以下测试的解锁地区是准确的，但是不是完整解锁的判断可能有误，这方面仅作参考使用
Youtube
[IPv4]
连接方式: Youtube Video Server
视频缓存节点地域: 德国法兰克福(FRA15S37)
Youtube识别地域: 无信息(null)

[IPv6]
连接方式: Youtube Video Server
视频缓存节点地域: 德国法兰克福(FRA15S37)
Youtube识别地域: 无信息(null)
Netflix
[IPv4]
您的出口IP可以使用Netflix，但仅可看Netflix自制剧
NF所识别的IP地域信息：德国
[IPv6]
您的出口IP可以使用Netflix，但仅可看Netflix自制剧
NF所识别的IP地域信息：德国
DisneyPlus
[IPv4]
当前IPv4出口解锁DisneyPlus
区域：德国区

[IPv6]
当前IPv6出口解锁DisneyPlus
区域：德国区
解锁Youtube，Netflix，DisneyPlus上面和下面进行比较，不同之处自行判断
---------------流媒体解锁--感谢RegionRestrictionCheck开源-------------
 以下为IPV4网络测试，若无IPV4网络则无输出
============[ Multination ]============
 Dazn:                                  No
 HotStar:                               No
 Disney+:                               No
 Netflix:                               Originals Only
 YouTube Premium:                       Yes (Region: DE)
 Amazon Prime Video:                    Yes (Region: DE)
 TVBAnywhere+:                          Yes
 iQyi Oversea Region:                   DE
 Viu.com:                               No
 YouTube CDN:                           Frankfurt 
 Netflix Preferred CDN:                 Amsterdam  
 Spotify Registration:                  No
 Steam Currency:                        EUR
=======================================
 以下为IPV6网络测试，若无IPV6网络则无输出
============[ Multination ]============
 Dazn:                                  Failed (Network Connection)
 HotStar:                               No
 Disney+:                               No
 Netflix:                               Originals Only
 YouTube Premium:                       Yes (Region: DE)
 Amazon Prime Video:                    Unsupported
 TVBAnywhere+:                          Failed (Network Connection)
 iQyi Oversea Region:                   Failed
 Viu.com:                               Failed
 YouTube CDN:                           Frankfurt 
 Netflix Preferred CDN:                 Amsterdam  
 Spotify Registration:                  No
 Steam Currency:                        Failed (Network Connection)
=======================================
-------------TikTok解锁--感谢lmc999加密脚本及fscarmen PR--------------
 Tiktok Region:         Failed
-----------------欺诈分数以及IP质量检测--本频道原创-------------------
以下仅作参考，不代表100%准确，如果和实际情况不一致请手动查询多个数据库比对
欺诈分数(越低越好)：32
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
2023/01/23 12:42:29 北京电信 219.141.136.12  电信163 [普通线路]           
2023/01/23 12:42:29 北京联通 202.106.50.1    联通4837[普通线路]           
2023/01/23 12:42:29 北京移动 221.179.155.161 移动CMI [普通线路]           
2023/01/23 12:42:29 上海电信 202.96.209.133  电信163 [普通线路]           
2023/01/23 12:42:29 上海联通 210.22.97.1     联通4837[普通线路]           
2023/01/23 12:42:29 上海移动 211.136.112.200 移动CMI [普通线路]           
2023/01/23 12:42:29 广州电信 58.60.188.222   电信163 [普通线路]           
2023/01/23 12:42:29 广州联通 210.21.196.6    联通4837[普通线路]           
2023/01/23 12:42:29 广州移动 120.196.165.24  移动CMI [普通线路]           
2023/01/23 12:42:29 成都电信 61.139.2.69     电信163 [普通线路]           
2023/01/23 12:42:29 成都联通 119.6.6.6       联通4837[普通线路]           
2023/01/23 12:42:29 成都移动 211.137.96.205  测试超时
------------------回程路由--感谢fscarmen开源及PR----------------------
IPv4 ASN: Hetzner Online GmbH
IPv6 ASN: Hetzner Online GmbH
依次测试电信，联通，移动经过的地区及线路，核心程序来由: ipip.net ，请知悉!
广州电信 58.60.188.222
5.19 ms  *  局域网
0.26 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
2.44 ms  AS24940  德国, 巴伐利亚州, 纽伦堡, hetzner.com
0.41 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
4.50 ms  AS24940  德国, 巴伐利亚州, 纽伦堡, hetzner.com
3.49 ms  AS1299  德国, 巴伐利亚州, 纽伦堡, telia.com
6.14 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
5.99 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
6.96 ms  AS4134  德国, 黑森州, 法兰克福, chinatelecom.com.cn, 电信
275.69 ms  AS134774  中国, 广东, 深圳, chinatelecom.com.cn, 电信
271.80 ms  AS4134  中国, 广东, 深圳, chinatelecom.com.cn, 电信
广州联通 210.21.196.6
6.30 ms  *  局域网
0.64 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
1.15 ms  AS24940  德国, 巴伐利亚州, 纽伦堡, hetzner.com
0.75 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
3.17 ms  AS24940  德国, 巴伐利亚州, 纽伦堡, hetzner.com
5.87 ms  AS1299  德国, 巴伐利亚州, 纽伦堡, telia.com
5.90 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
6.36 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
163.97 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
179.32 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
174.63 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
164.71 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
广州移动 120.196.165.2
4.80 ms  *  局域网
0.61 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
1.59 ms  AS24940  德国, 巴伐利亚州, 纽伦堡, hetzner.com
6.27 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
5.39 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
14.96 ms  *  德国, 黑森州, 法兰克福, de-cix.net
6.74 ms  AS58453  德国, 黑森州, 法兰克福, chinamobile.com, 移动
229.04 ms  AS58453  中国, 上海, chinamobile.com, 移动
256.01 ms  AS58453  中国, 广东, 广州, chinamobile.com, 移动
263.42 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
266.05 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
271.27 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
279.42 ms  AS56040  中国, 广东, 深圳, chinamobile.com, 移动
--------网络测速--由teddysun和superspeed开源及spiritlhls整理----------
测速点位置       上传速度        下载速度        延迟
Speedtest.net    0.85 Mbps       0.72 Mbps       121.02 ms
洛杉矶           579.88 Mbps     3635.41 Mbps    158.89 ms
新加坡           60.36 Mbps      1977.79 Mbps    169.74 ms
中国香港         459.51 Mbps     995.65 Mbps     198.56 ms
电信上海         1.04 Mbps       1657.03 Mbps    255.06 ms
电信广东广州5G   1.11 Mbps       212.39 Mbps     267.95 ms
联通上海         65.41 Mbps      1819.92 Mbps    228.03 ms
联通湖南长沙     135.23 Mbps     1180.54 Mbps    167.09 ms
移动广西南宁     351.56 Mbps     942.30 Mbps     182.74 ms
----------------------------------------------------------------------
 总共花费      : 7 分 26 秒
 时间          : Mon 23 Jan 2023 12:48:27 PM UTC
----------------------------------------------------------------------
```

## 网络测试

Speedtest有那么一点点小Bug

![](https://www.speedtest.net/result/c/b14bb8c6-3d49-4e2d-b6c4-da38e0ebd30d.png)

流媒体图一乐呵

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_01-23_21-36-22.png)

国内测速还能看

```
——————————————————————————————————————————————————————————
ID    测速服务器信息       上传/Mbps   下载/Mbps   延迟/ms
17145 电信|安徽合肥５Ｇ　　↑ 1.69      ↓ 1095.51   248.84  
27594 电信|广东广州５Ｇ　　↑ 2.62      ↓ 251.47    288.11  
5396  电信|江苏苏州５Ｇ　　↑ 1.95      ↓ 990.84    279.50  
23844 电信|湖北武汉　　　　↑ 11.45     ↓ 46.26     254.67  
29353 电信|湖北武汉５Ｇ　　↑ 1.98      ↓ 110.89    254.22  
28225 电信|湖南长沙５Ｇ　　↑ 1.80      ↓ 620.87    263.31  
3973  电信|甘肃兰州　　　　↑ 54.65     ↓ 30.44     597.71  
24447 联通|上海５Ｇ　　　　↑ 3.22      ↓ 1592.35   228.95  
4870  联通|湖南长沙　　　　↑ 5.27      ↓ 1301.26   159.62  
25858 移动|北京　　　　　　↑ 422.95    ↓ 1075.04   304.58  
——————————————————————————————————————————————————————————
```

## 结论

整体来说还是不错的，测试问题有可能是测速节点的Bug，风控相较于OVH和NC比较松，做点正常站没啥问题。
