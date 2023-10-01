## 风险预警

域名2021注册，2022正式开业的美国商家，能刷卡/PayPal。不建议用于生产环境，用于刷PT，做下载机还行。

~~（感觉有国人倾向，下午北京时间三点秒回工单装硬盘）~~

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_01-24_16-16-22.png)

## 价格

[官网传送门](https://my.crunchbits.com/)

大盘鸡还是值得看看的，其他的感觉不是那么实惠。最低配大盘鸡有优惠码，首月4.8刀，自己去LOC找找看，这里就不放了。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_01-24_16-30-10.png)

下单后只有7GB SSD，需要手动开个工单找客服挂载HDD硬盘。据说流量超后不会停机，而是限速到5Mbps。用的virtfusion面板，下单后自己去装系统，开启IPv6。

挂载硬盘的教程可以看看我以前写的文章：[传送门](https://www.gakiyukr.net/archives/283)

## 性能测试

洋垃圾E5+石头盘，不过嘛，毕竟这个价了，要求不能太高。

```
-------------------- A Bench Script By spiritlhl ---------------------
                   测评频道: https://t.me/vps_reviews                    
版本：2023.01.20
更新日志：融合怪九代目(集合百家之长)(专为测评频道小鸡而生)
-----------------感谢teddysun和superbench和yabs开源-------------------
 CPU 型号          : Intel(R) Xeon(R) CPU E5-2695 v4 @ 2.10GHz
 CPU 核心数        : 1
 CPU 频率          : 2095.148 MHz
 CPU 缓存          : 46080 KB
 硬盘空间          : 6.9 GB (1.5 GB 已用)
 内存              : 943 MB (124 MB 已用)
 Swap              : 0 MB (0 MB 已用)
 系统在线时间      : 0 days, 0 hour 10 min
 负载              : 0.59, 0.37, 0.27
 系统              : Debian GNU/Linux 11 (bullseye)
 AES-NI指令集      : ✔ Enabled
 VM-x/AMD-V支持    : ✔ Enabled
 架构              : x86_64 (64 Bit)
 内核              : 5.10.0-10-amd64
 TCP加速方式       : cubic
 虚拟化架构        : KVM
 ASN组织           : AS400304 REDOUBT NETWORKS
 位置              : Spokane / US
 地区              : Washington
-------------------CPU测试--感谢lemonbench开源------------------------
 -> CPU 测试中 (Fast Mode, 1-Pass @ 5sec)
 1 线程测试(1核)得分:           783 Scores
-------------------内存测试--感谢lemonbench开源-----------------------
 -> 内存测试 Test (Fast Mode, 1-Pass @ 5sec)
 单线程读测试:          16302.93 MB/s
 单线程写测试:          11149.19 MB/s
----------------磁盘IO读写测试--感谢lemonbench开源--------------------
 -> 磁盘IO测试中 (4K Block/1M Block, Direct Mode)
 测试操作               写速度                                  读速度
 100MB-4K Block         17.8 MB/s (4338 IOPS, 5.90s)            14.2 MB/s (3472 IOPS, 7.37s)
 1GB-1M Block           209 MB/s (199 IOPS, 5.02s)              128 MB/s (122 IOPS, 8.16s)
-------------------磁盘IO读写测试--感谢yabs开源-----------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 44.85 MB/s   (11.2k) | 67.56 MB/s    (1.0k)
Write      | 44.91 MB/s   (11.2k) | 67.96 MB/s    (1.0k)
Total      | 89.77 MB/s   (22.4k) | 135.53 MB/s   (2.1k)           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 95.49 MB/s     (186) | 97.35 MB/s      (95)
Write      | 100.56 MB/s    (196) | 103.83 MB/s    (101)
Total      | 196.05 MB/s    (382) | 201.19 MB/s    (196)
--------------------流媒体解锁--感谢sjlleo开源------------------------
以下测试的解锁地区是准确的，但是不是完整解锁的判断可能有误，这方面仅作参考使用
Youtube
[IPv4]
连接方式: Youtube Video Server
视频缓存节点地域: 美国  西雅图(SEA09S34)
Youtube识别地域: 无信息(null)

[IPv6]
连接方式: Youtube Video Server
视频缓存节点地域: 美国  西雅图(SEA09S34)
Youtube识别地域: 无信息(null)
Netflix
[IPv4]
您的出口IP完整解锁Netflix，支持非自制剧的观看
NF所识别的IP地域信息：美国
[IPv6]
您的出口IP完整解锁Netflix，支持非自制剧的观看
NF所识别的IP地域信息：美国
DisneyPlus
[IPv4]
当前IPv4出口解锁DisneyPlus
区域：美国区

[IPv6]
当前IPv6出口解锁DisneyPlus
区域：美国区
解锁Youtube，Netflix，DisneyPlus上面和下面进行比较，不同之处自行判断
---------------流媒体解锁--感谢RegionRestrictionCheck开源-------------
 以下为IPV4网络测试，若无IPV4网络则无输出
============[ Multination ]============
 Dazn:                                  No
 HotStar:                               Yes (Region: US)
 Disney+:                               Yes (Region: US)
 Netflix:                               Yes (Region: US)
 YouTube Premium:                       Yes
 Amazon Prime Video:                    Yes (Region: US)
 TVBAnywhere+:                          Yes
 iQyi Oversea Region:                   US
 Viu.com:                               No
 YouTube CDN:                           Seattle, WA 
 Netflix Preferred CDN:                 Seattle, WA  
 Spotify Registration:                  Yes (Region: US)
 Steam Currency:                        USD
=======================================
 以下为IPV6网络测试，若无IPV6网络则无输出
============[ Multination ]============
 Dazn:                                  Failed (Network Connection)
 HotStar:                               Yes (Region: US)
 Disney+:                               Yes (Region: US)
 Netflix:                               Yes (Region: US)
 YouTube Premium:                       Yes
 Amazon Prime Video:                    Unsupported
 TVBAnywhere+:                          Failed (Network Connection)
 iQyi Oversea Region:                   Failed
 Viu.com:                               Failed
 YouTube CDN:                           Seattle, WA 
 Netflix Preferred CDN:                 Seattle, WA  
 Spotify Registration:                  Yes (Region: US)
 Steam Currency:                        Failed (Network Connection)
=======================================
-------------TikTok解锁--感谢lmc999加密脚本及fscarmen PR--------------
 Tiktok Region:         【US】
-----------------欺诈分数以及IP质量检测--本频道原创-------------------
以下仅作参考，不代表100%准确，如果和实际情况不一致请手动查询多个数据库比对
欺诈分数(越低越好)：89
匿名代理: No
Tor出口节点: No
服务器IP: No
公共代理: No
网络代理: No
搜索引擎机器人: No
abuse得分： 0
IP2Location数据库IP类型： Commercial
ping0数据库IP类型：IDC机房IP
Google搜索可行性：YES
-----------------三网回程--感谢zhanghanyun/backtrace开源--------------
2023/01/24 16:18:31 北京电信 219.141.136.12  测试超时
2023/01/24 16:18:31 北京联通 202.106.50.1    测试超时
2023/01/24 16:18:31 北京移动 221.179.155.161 测试超时
2023/01/24 16:18:31 上海电信 202.96.209.133  测试超时
2023/01/24 16:18:31 上海联通 210.22.97.1     测试超时
2023/01/24 16:18:31 上海移动 211.136.112.200 测试超时
2023/01/24 16:18:31 广州电信 58.60.188.222   测试超时
2023/01/24 16:18:31 广州联通 210.21.196.6    测试超时
2023/01/24 16:18:31 广州移动 120.196.165.24  测试超时
2023/01/24 16:18:31 成都电信 61.139.2.69     测试超时
2023/01/24 16:18:31 成都联通 119.6.6.6       联通4837[普通线路]           
2023/01/24 16:18:31 成都移动 211.137.96.205  测试超时
------------------回程路由--感谢fscarmen开源及PR----------------------
IPv4 ASN: Redoubt Networks LLC
IPv6 ASN: Redoubt Networks LLC
依次测试电信，联通，移动经过的地区及线路，核心程序来由: ipip.net ，请知悉!
广州电信 58.60.188.222
0.56 ms  AS400304  美国, 爱达荷州, 科达伦, redoubtnet.com
1.21 ms  AS964  美国, 爱达荷州, 科达伦, ionswitch.com
1.19 ms  AS20055  美国, 爱达荷州, 科达伦, ziplyfiber.com
11.58 ms  AS20055  美国, 爱达荷州, 科达伦, ziplyfiber.com
11.79 ms  AS20055  美国, 华盛顿州, 普尔曼, ziplyfiber.com
11.68 ms  AS20055  美国, 华盛顿州, 肯纳威克, ziplyfiber.com
11.69 ms  AS20055  美国, 华盛顿州, 肯纳威克, ziplyfiber.com
11.75 ms  AS20055  美国, 华盛顿州, 肯纳威克, ziplyfiber.com
11.81 ms  AS20055  美国, 华盛顿州, 亚基马, ziplyfiber.com
12.00 ms  AS20055  美国, 华盛顿州, 亚基马, ziplyfiber.com
11.53 ms  AS20055  美国, 华盛顿州, 西雅图, ziplyfiber.com
11.23 ms  AS6461  美国, 华盛顿州, 西雅图, zayo.com
31.89 ms  AS6461  美国, 加利福尼亚州, 圣何塞, zayo.com
30.39 ms  AS6461  美国, 加利福尼亚州, 圣何塞, zayo.com
245.90 ms  AS4134  中国, 广东, 广州, chinatelecom.com.cn, 电信
262.32 ms  AS134774  中国, 广东, 深圳, chinatelecom.com.cn, 电信
249.06 ms  AS4134  中国, 广东, 深圳, chinatelecom.com.cn, 电信
广州联通 210.21.196.6
0.33 ms  AS400304  美国, 爱达荷州, 科达伦, redoubtnet.com
0.94 ms  AS964  美国, 爱达荷州, 科达伦, ionswitch.com
1.12 ms  AS20055  美国, 爱达荷州, 科达伦, ziplyfiber.com
11.85 ms  AS20055  美国, 爱达荷州, 科达伦, ziplyfiber.com
12.05 ms  AS20055  美国, 华盛顿州, 普尔曼, ziplyfiber.com
11.84 ms  AS20055  美国, 华盛顿州, 肯纳威克, ziplyfiber.com
12.15 ms  AS20055  美国, 华盛顿州, 肯纳威克, ziplyfiber.com
11.83 ms  AS20055  美国, 华盛顿州, 肯纳威克, ziplyfiber.com
12.02 ms  AS20055  美国, 华盛顿州, 亚基马, ziplyfiber.com
11.62 ms  AS20055  美国, 华盛顿州, 西雅图, ziplyfiber.com
11.54 ms  AS20055  美国, 华盛顿州, 西雅图, ziplyfiber.com
11.93 ms  AS174  美国, 华盛顿州, 西雅图, cogentco.com
32.11 ms  AS174  美国, 犹他州, 盐湖城, cogentco.com
46.29 ms  AS174  美国, 加利福尼亚州, 旧金山, cogentco.com
47.56 ms  AS174  美国, 加利福尼亚州, 圣何塞, cogentco.com
59.46 ms  AS174  美国, 加利福尼亚州, 洛杉矶, cogentco.com
59.81 ms  AS174  美国, 加利福尼亚州, 洛杉矶, cogentco.com
52.18 ms  AS174  美国, 加利福尼亚州, 洛杉矶, cogentco.com
220.01 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
221.15 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
259.14 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
235.54 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
广州移动 120.196.165.2
0.28 ms  AS400304  美国, 爱达荷州, 科达伦, redoubtnet.com
0.89 ms  AS964  美国, 爱达荷州, 科达伦, ionswitch.com
0.89 ms  AS20055  美国, 爱达荷州, 科达伦, ziplyfiber.com
11.47 ms  AS20055  美国, 爱达荷州, 科达伦, ziplyfiber.com
11.42 ms  AS20055  美国, 华盛顿州, 普尔曼, ziplyfiber.com
11.42 ms  AS20055  美国, 华盛顿州, 肯纳威克, ziplyfiber.com
11.73 ms  AS20055  美国, 华盛顿州, 肯纳威克, ziplyfiber.com
11.82 ms  AS20055  美国, 华盛顿州, 肯纳威克, ziplyfiber.com
11.83 ms  AS20055  美国, 华盛顿州, 肯纳威克, ziplyfiber.com
11.09 ms  AS20055  美国, 俄勒冈州, 比弗顿, ziplyfiber.com
11.05 ms  AS20055  美国, 俄勒冈州, 比弗顿, ziplyfiber.com
11.31 ms  AS20055  美国, 俄勒冈州, 希尔斯伯勒, ziplyfiber.com
11.46 ms  AS20055  美国, 俄勒冈州, 希尔斯伯勒, ziplyfiber.com
11.25 ms  AS20055  美国, 俄勒冈州, 希尔斯伯勒, ziplyfiber.com
10.89 ms  AS1299  美国, 俄勒冈州, 波特兰, telia.com
11.23 ms  AS1299  美国, 俄勒冈州, 波特兰, telia.com
13.62 ms  AS1299  美国, 华盛顿州, 西雅图, telia.com
19.18 ms  AS1299  美国, 华盛顿州, 西雅图, telia.com
214.22 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
212.73 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
222.52 ms  AS56040  中国, 广东, 深圳, chinamobile.com, 移动
--------网络测速--由teddysun和superspeed开源及spiritlhls整理----------
测速点位置       上传速度        下载速度        延迟
Speedtest.net    947.68 Mbps     945.98 Mbps     51.51 ms
洛杉矶           1001.20 Mbps    943.03 Mbps     37.33 ms
新加坡           174.05 Mbps     650.00 Mbps     236.77 ms
中国香港         497.79 Mbps     739.08 Mbps     173.95 ms
电信上海         288.86 Mbps     782.81 Mbps     163.58 ms
电信广东广州5G   8.05 Mbps       298.68 Mbps     190.64 ms
联通上海         336.48 Mbps     727.51 Mbps     282.64 ms
联通湖南长沙     1.61 Mbps       584.80 Mbps     246.98 ms
移动广西南宁     525.03 Mbps     942.50 Mbps     105.91 ms
移动宁夏银川     1.32 Mbps       692.83 Mbps     235.75 ms
----------------------------------------------------------------------
 总共花费      : 10 分 22 秒
 时间          : Tue 24 Jan 2023 04:25:11 PM HKT
----------------------------------------------------------------------
```

## 网络测试

G口，国内连通性图一乐。

![](https://www.speedtest.net/result/c/5a0ddf98-390e-497d-a230-0f77860fac8f.png)

```
——————————————————————————————————————————————————————————
ID    测速服务器信息       上传/Mbps   下载/Mbps   延迟/ms
3633  电信|上海　　　　　　↑ 261.17    ↓ 2.08      223.74  
17145 电信|安徽合肥５Ｇ　　↑ 154.99    ↓ 1.16      229.66  
27594 电信|广东广州５Ｇ　　↑ 225.30    ↓ 0.59      244.23  
5396  电信|江苏苏州５Ｇ　　↑ 1038.36   ↓ 6.44      235.43  
23844 电信|湖北武汉　　　　↑ 453.21    ↓ 673.55    187.20  
29353 电信|湖北武汉５Ｇ　　↑ 449.01    ↓ 676.26    184.35  
28225 电信|湖南长沙５Ｇ　　↑ 1072.78   ↓ 471.53    197.50  
3973  电信|甘肃兰州　　　　↑ 6.20      ↓ 681.29    195.31  
24447 联通|上海５Ｇ　　　　↑ 526.24    ↓ 635.14    283.09  
4870  联通|湖南长沙　　　　↑ 78.86     ↓ 546.63    229.45  
25858 移动|北京　　　　　　↑ 26.04     ↓ 971.29    302.76  
——————————————————————————————————————————————————————————
```

这洋垃圾解锁流媒体，还是非常意外的。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_01-24_18-00-34.png)

## 结语

整体来说有点意思，可以有保种需求可以买一台~~（顺便搞个节点看流媒体）~~，跑业务就算了，新商家。