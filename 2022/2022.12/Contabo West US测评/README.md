Contabo，超售小王子，4C8G当2C4G用就行。

记得改成EUR付款，便宜很多钱。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-06_08-21-50.png)

本次测评的是5.99 EUR（4C8C）款的美西机房，正常情况下该机房需要每个月+1.45EUR，黑五活动免费了。有200G SSD或者是50G NVMe可选，32TB出站+无限入站，200Mbps带宽。

正常价格还需要安装费（是的，vps都收安装费）年付可免安装费。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-06_08-26-02.png)

这家只建议在黑五等活动购买，有硬盘翻倍，免安装费，免地区费活动。正价11.98EUR还是很贵的。

**注意：这鸟玩意大概率要KYC的，我两个号第一次下单都触发了KYC验证。**提交身份证+云闪付交易记录截图就过了~~（这鸟玩意大概率有国人员工或者是国人商家？）~~

## 配置

很奇怪的是，IP被识别为捷克和德国，但是看路由发现还是在西雅图。

```
--------------------- A Bench Script By spiritlhl ---------------------
                   测评频道: https://t.me/vps_reviews                    
版本：2022.11.28
更新日志：融合怪九代目(集合百家之长)(专为测评频道小鸡而生)
-----------------感谢teddysun和misakabench和yabs开源-------------------
 CPU 型号          : AMD EPYC 7282 16-Core Processor
 CPU 核心数        : 4
 CPU 频率          : 2794.750 MHz
 CPU 缓存          : 512 KB
 硬盘空间          : 196.0 GB (22.1 GB 已用)
 内存              : 7951 MB (3281 MB 已用)
 Swap              : 0 MB (0 MB 已用)
 系统在线时间      : 9 days, 10 hour 57 min
 负载              : 0.40, 0.19, 0.11
 系统              : Ubuntu 22.04.1 LTS
 AES-NI指令集      : ✔ Enabled
 VM-x/AMD-V支持    : ❌ Disabled
 架构              : x86_64 (64 Bit)
 内核              : 5.15.0-25-generic
 TCP加速方式       : cubic
 虚拟化架构        : Dedicated
 ASN组织           : AS40021 Contabo Inc.
 位置              : Munich / DE
 地区              : Bavaria
-------------------CPU测试--感谢lemonbench开源------------------------
 -> CPU 测试中 (Fast Mode, 1-Pass @ 5sec)
 1 线程测试(1核)得分:           1556 Scores
 4 线程测试(多核)得分:          6030 Scores
-------------------内存测试--感谢lemonbench开源-----------------------
 -> 内存测试 Test (Fast Mode, 1-Pass @ 5sec)
 单线程读测试:          39691.82 MB/s
 单线程写测试:          17128.27 MB/s
----------------磁盘IO读写测试--感谢lemonbench开源--------------------
 -> 磁盘IO测试中 (4K Block/1M Block, Direct Mode)
 测试操作               写速度                                  读速度
 100MB-4K Block         6.7 MB/s (1638 IOPS, 15.62s)            45.2 MB/s (11031 IOPS, 2.32s)
 1GB-1M Block           210 MB/s (199 IOPS, 5.00s)              2.0 GB/s (1871 IOPS, 0.53s)
-------------------磁盘IO读写测试--感谢yabs开源-----------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 5.30 MB/s     (1.3k) | 64.11 MB/s    (1.0k)
Write      | 5.32 MB/s     (1.3k) | 64.53 MB/s    (1.0k)
Total      | 10.62 MB/s    (2.6k) | 128.65 MB/s   (2.0k)           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 127.62 MB/s    (249) | 97.50 MB/s      (95)
Write      | 134.40 MB/s    (262) | 103.99 MB/s    (101)
Total      | 262.02 MB/s    (511) | 201.49 MB/s    (196)
--------------------流媒体解锁--感谢sjlleo开源-------------------------
以下测试的解锁地区是准确的，但是不是完整解锁的判断可能有误，这方面仅作参考使用
Youtube
[IPv4]
连接方式: Youtube Video Server
视频缓存节点地域: ORD(ORD38S15)
Youtube识别地域: 无信息(null)
Netflix
[IPv4]
您的出口IP可以使用Netflix，但仅可看Netflix自制剧
NF所识别的IP地域信息：捷克
[IPv6]
您的网络可能没有正常配置IPv6，或者没有IPv6网络接入
DisneyPlus
[IPv4]
当前IPv4出口解锁DisneyPlus
区域：捷克区
解锁Youtube，Netflix，DisneyPlus的地区以上面为准，下面这三测的不准
---------------流媒体解锁--感谢RegionRestrictionCheck开源-------------
 以下为IPV4网络测试
============[ Multination ]============
 Dazn:                                  Unsupport
 HotStar:                               No
 Disney+:                               No
 Netflix:                               Originals Only
 YouTube Premium:                       Yes
 Amazon Prime Video:                    Yes (Region: CZ)
 TVBAnywhere+:                          Failed
 iQyi Oversea Region:                   INTL
 Viu.com:                               No
 YouTube CDN:                           Chicago, IL 
 Netflix Preferred CDN:                 Associated with [] in [Washington DC ]
 Steam Currency:ation:                  USDSteam Currency:                      ->
=======================================
 以下为IPV6网络测试
============[ Multination ]============
 Dazn:                                  Failed (Network Connection)
 HotStar:                               Failed (Network Connection)
 Disney+:                               No
 Netflix:                               Failed (Network Connection)
 YouTube Premium:                       Failed (Network Connection)
 Amazon Prime Video:                    Unsupported
 TVBAnywhere+:                          Failed (Network Connection)
 iQyi Oversea Region:                   Failed
 Viu.com:                               Failed
 YouTube Region:                        Check Failed (Network Connection)
 Netflix Preferred CDN:                 Failed
 Steam Currency:ation:                  Failed (Network Connection)             ->
=======================================
---------------TikTok解锁--感谢superbench的开源脚本----------------
 TikTok               : Yes (Region: CZ)
------------------欺诈分数以及IP质量检测--本频道原创-------------------
得分仅作参考，不代表100%准确
欺诈分数(越低越好)：31
匿名代理: No
Tor出口节点: No
服务器IP: Yes
公共代理: No
网络代理: No
搜索引擎机器人: No
IP类型： Data Center/Web Hosting/Transit
abuse得分： 0
Google搜索可行性：yes
-----------------三网回程--感谢zhanghanyun/backtrace开源--------------
2022/12/05 15:33:32 正在测试三网回程路由...
2022/12/05 15:33:33 北京电信 219.141.136.12  测试超时
2022/12/05 15:33:33 北京联通 202.106.50.1    联通4837[普通线路]
2022/12/05 15:33:33 北京移动 221.179.155.161 移动CMI [普通线路]
2022/12/05 15:33:33 上海电信 202.96.209.133  测试超时
2022/12/05 15:33:33 上海联通 210.22.97.1     联通4837[普通线路]
2022/12/05 15:33:33 上海移动 211.136.112.200 移动CMI [普通线路]
2022/12/05 15:33:33 广州电信 58.60.188.222   电信163 [普通线路]
2022/12/05 15:33:33 广州联通 210.21.196.6    联通4837[普通线路]
2022/12/05 15:33:33 广州移动 120.196.165.24  移动CMI [普通线路]
------------------回程路由--感谢fscarmen开源及PR----------------------
以下测试的带宽类型可能有误，商宽可能被判断为家宽，仅作参考使用
依次测试电信，联通，移动经过的地区及线路，核心程序来由: ipip.net ，请知悉!
广州电信 58.60.188.222
0.92 ms  AS40021  美国, 华盛顿州, 西雅图, contabo.com
1.59 ms  AS3356  美国, 华盛顿州, 西雅图, level3.com
23.22 ms  AS3356  美国, 加利福尼亚州, 圣何塞, level3.com
25.83 ms  AS3356  美国, 加利福尼亚州, 圣何塞, level3.com
165.45 ms  AS4134  中国, 广东, 广州, chinatelecom.com.cn, 电信
168.20 ms  AS4134  中国, 广东, 广州, chinatelecom.com.cn, 电信
172.19 ms  AS134774  中国, 广东, 深圳, chinatelecom.com.cn, 电信
173.93 ms  AS4134  中国, 广东, 深圳, chinatelecom.com.cn, 电信
广州联通 210.21.196.6
0.50 ms  AS40021  美国, 华盛顿州, 西雅图, contabo.com
1.79 ms  *  局域网
9.38 ms  AS3356  美国, 华盛顿州, 西雅图, level3.com
33.00 ms  AS3356  美国, 加利福尼亚州, 洛杉矶, level3.com
186.90 ms  AS3356  美国, 加利福尼亚州, 洛杉矶, level3.com
215.34 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
184.05 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
229.20 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
184.13 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
广州移动 120.196.165.2
0.56 ms  AS40021  美国, 华盛顿州, 西雅图, contabo.com
1.55 ms  *  局域网
1.51 ms  AS3356  美国, 华盛顿州, 西雅图, level3.com
20.50 ms  AS3356  美国, 华盛顿州, 西雅图, level3.com
19.74 ms  AS58453  美国, 华盛顿州, 西雅图, chinamobile.com, 移动
161.74 ms  AS58453  中国, 广东, 广州, chinamobile.com, 移动
174.14 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
163.98 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
171.16 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
175.66 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
173.12 ms  AS56040  中国, 广东, 广州, chinamobile.com, 移动
169.54 ms  AS56040  中国, 广东, 深圳, chinamobile.com, 移动
--------网络测速--由teddysun和superspeed开源及spiritlhls整理----------
测速点位置       上传速度        下载速度        延迟
speedtest        190.99 Mbps     200.13 Mbps     1.06 ms
洛杉矶  　　　   190.92Mbps      199.51Mbps      33.93ms
新加坡  　　　   188.92Mbps      200.11Mbps      210.87ms
日本东京　　�    190.83Mbps      202.23Mbps      105.50ms
中国香港　　�    192.69Mbps      0.32Mbps        171.12ms
电信上海　　�    193.00Mbps      204.11Mbps      164.37ms
电信广东广州5G   48.38Mbps       161.35Mbps      181.71ms
联通上海　　�    186.34Mbps      203.88Mbps      152.42ms
联通湖南长沙�    193.28Mbps      202.25Mbps      168.49ms
----------------------------------------------------------------------
 总共花费        : 8 分 19 秒
 时间          : Mon Dec  5 15:38:37 PST 2022
----------------------------------------------------------------------
ID    测速服务器信息       上传/Mbps   下载/Mbps   延迟/ms
3633  电信|上海　　　　　　↑ 189.11    ↓ 207.18    154.12  
17145 电信|安徽合肥５Ｇ　　↑ 167.41    ↓ 204.96    161.49  
27594 电信|广东广州５Ｇ　　↑ 85.10     ↓ 192.94    213.69  
5396  电信|江苏苏州５Ｇ　　↑ 185.35    ↓ 208.98    148.51  
23844 电信|湖北武汉　　　　↑ 172.66    ↓ 204.85    164.51  
29353 电信|湖北武汉５Ｇ　　↑ 172.67    ↓ 205.23    161.29  
28225 电信|湖南长沙５Ｇ　　↑ 182.66    ↓ 203.46    185.38  
3973  电信|甘肃兰州　　　　↑ 56.82     ↓ 110.71    193.84  
24447 联通|上海５Ｇ　　　　↑ 192.86    ↓ 205.93    153.31  
4870  联通|湖南长沙　　　　↑ 186.51    ↓ 196.07    169.22  
25858 移动|北京　　　　　　↑ 179.59    ↓ 197.59    215.40 
```

![](https://s3-jp-ap-3.040407.xyz/oss/photos/contusping.png)

G5单核813分：[传送门](https://browser.geekbench.com/v5/cpu/19113529)

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-06_09-27-47.png)

## 总结

整体来说还是看得过去的，比德国机房稍微好点，当然这家本身的问题就不少，比如说没法dd，安装费，超售等，建议活动买台玩玩得了，不建议用于生产业务。