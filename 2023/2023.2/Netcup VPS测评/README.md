Netcup老牌德国厂商，关于他的介绍可以看我写的[另一篇文章](https://www.gakiyukr.net/archives/326)，这里就一笔带过了。
本次测评的型号是VPS 200 G10s，3.25EUR（不计算VAT）/月

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_02-18_22-02-37.png)


```
-------------------- A Bench Script By spiritlhl ---------------------
                   测评频道: https://t.me/vps_reviews                    
版本：2023.02.11
更新日志：融合怪九代目(集合百家之长)(专为测评频道小鸡而生)
-----------------感谢teddysun和superbench和yabs开源-------------------
 CPU 型号          : QEMU Virtual CPU version 2.5+
 CPU 核心数        : 2
 CPU 频率          : 1996.248 MHz
 CPU 缓存          : 512 KB
 硬盘空间          : 40.0 GB (1.4 GB 已用)
 内存              : 1995 MB (57 MB 已用)
 Swap              : 0 MB (0 MB 已用)
 系统在线时间      : 0 days, 0 hour 7 min
 负载              : 0.06, 0.02, 0.00
 系统              : Debian GNU/Linux 10 (buster)
 AES-NI指令集      : ✔ Enabled
 VM-x/AMD-V支持    : ❌ Disabled
 架构              : x86_64 (64 Bit)
 内核              : 4.19.0-23-amd64
 TCP加速方式       : cubic
 虚拟化架构        : KVM
 ASN组织           : AS197540 netcup GmbH
 位置              : Karlsruhe / DE
 地区              : Baden-Wurttemberg
-------------------CPU测试--感谢lemonbench开源------------------------
 -> CPU 测试中 (Fast Mode, 1-Pass @ 5sec)
 1 线程测试(1核)得分:           1407 Scores
 2 线程测试(多核)得分:          2364 Scores
-------------------内存测试--感谢lemonbench开源-----------------------
 -> 内存测试 Test (Fast Mode, 1-Pass @ 5sec)
 单线程读测试:          37298.27 MB/s
 单线程写测试:          16780.57 MB/s
----------------磁盘IO读写测试--感谢lemonbench开源--------------------
 -> 磁盘IO测试中 (4K Block/1M Block, Direct Mode)
 测试操作               写速度                                  读速度
 100MB-4K Block         35,9 MB/s (0.08 IOPS, 2.00s))           41,9 MB/s (12800 IOPS, 2.00s)
 1GB-1M Block           955 MB/s (1000 IOPS, 1.00s)             2,4 GB/s (2147483647 IOPS, 0.00s)
-------------------磁盘IO读写测试--感谢yabs开源-----------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 27.29 MB/s    (6.8k) | 289.58 MB/s   (4.5k)
Write      | 27.32 MB/s    (6.8k) | 291.10 MB/s   (4.5k)
Total      | 54.62 MB/s   (13.6k) | 580.68 MB/s   (9.0k)           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 960.90 MB/s   (1.8k) | 1.65 GB/s     (1.6k)
Write      | 1.01 GB/s     (1.9k) | 1.76 GB/s     (1.7k)
Total      | 1.97 GB/s     (3.8k) | 3.42 GB/s     (3.3k)
--------------------流媒体解锁--感谢sjlleo开源------------------------
以下测试的解锁地区是准确的，但是不是完整解锁的判断可能有误，这方面仅作参考使用
----------------Youtube----------------
[IPv4]
连接方式: Google Global CacheCDN (ISP Cooperation)
ISP运营商: ANEXIAAT
视频缓存节点地域: 奥地利维也纳(VIE1)
Youtube识别地域: 无信息(null)
[IPv6]
连接方式: Google Global CacheCDN (ISP Cooperation)
ISP运营商: ANEXIAAT
视频缓存节点地域: 奥地利维也纳(VIE1)
Youtube识别地域: 无信息(null)
----------------Netflix----------------
[IPv4]
您的出口IP可以使用Netflix，但仅可看Netflix自制剧
NF所识别的IP地域信息：德国
[IPv6]
您的出口IP可以使用Netflix，但仅可看Netflix自制剧
NF所识别的IP地域信息：德国
---------------DisneyPlus---------------
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
 HotStar:                               Failed (Network Connection)
 Disney+:                               Yes (Region: DE)
 Netflix:                               Originals Only
 YouTube Premium:                       Yes (Region: DE)
 Amazon Prime Video:                    Yes (Region: DE)
 TVBAnywhere+:                          Yes
 iQyi Oversea Region:                   DE
 Viu.com:                               No
 YouTube CDN:                           Associated with [ANEXIAAT]
 Netflix Preferred CDN:                 Associated with [Anexia] in [Vienna ]
 Spotify Registration:                  No
 Steam Currency:                        EUR
=======================================
 以下为IPV6网络测试，若无IPV6网络则无输出
============[ Multination ]============
 Dazn:                                  Failed (Network Connection)
 HotStar:                               Failed (Network Connection)
 Disney+:                               Yes (Region: DE)
 Netflix:                               Originals Only
 YouTube Premium:                       Yes (Region: DE)
 Amazon Prime Video:                    Unsupported
 TVBAnywhere+:                          Failed (Network Connection)
 iQyi Oversea Region:                   Failed
 Viu.com:                               Failed
 YouTube CDN:                           Associated with [ANEXIAAT]
 Netflix Preferred CDN:                 Associated with [Anexia] in [Vienna ]
 Spotify Registration:                  No
 Steam Currency:                        Failed (Network Connection)
=======================================
-------------TikTok解锁--感谢lmc999的源脚本及fscarmen PR--------------
 Tiktok Region:         【AT】
--------------OpenAi解锁--感谢missuo的OpenAI-Checker项目--------------
[IPv4]
Your IP supports access to OpenAI. Region: AT
[IPv6]
Your IP supports access to OpenAI. Region: DE
-----------------欺诈分数以及IP质量检测--本频道原创-------------------
以下仅作参考，不代表100%准确，如果和实际情况不一致请手动查询多个数据库比对
------以下为IPV4检测------
scamalytics数据库:
  欺诈分数(越低越好)：84
  匿名代理: No
  Tor出口节点: No
  服务器IP: Yes
  公共代理: No
  网络代理: No
  搜索引擎机器人: No
ip-api数据库:
  手机流量: No
  代理服务: No
  数据中心: Yes
abuseipdb数据库-abuse得分： 0
IP类型:
  IP2Location数据库:  Data Center/Web Hosting/Transit
  liveipmap数据库：(DCH) Data Center/Web Hosting/Transit
Google搜索可行性：未知
-----------------三网回程--感谢zhanghanyun/backtrace开源--------------
2023/02/17 07:38:59 北京电信 219.141.136.12  电信163 [普通线路]           
2023/02/17 07:38:59 北京联通 202.106.50.1    联通4837[普通线路]           
2023/02/17 07:38:59 北京移动 221.179.155.161 移动CMI [普通线路]           
2023/02/17 07:38:59 上海电信 202.96.209.133  电信163 [普通线路]           
2023/02/17 07:38:59 上海联通 210.22.97.1     联通4837[普通线路]           
2023/02/17 07:38:59 上海移动 211.136.112.200 移动CMI [普通线路]           
2023/02/17 07:38:59 广州电信 58.60.188.222   电信163 [普通线路]           
2023/02/17 07:38:59 广州联通 210.21.196.6    联通4837[普通线路]           
2023/02/17 07:38:59 广州移动 120.196.165.24  移动CMI [普通线路]           
2023/02/17 07:38:59 成都电信 61.139.2.69     电信163 [普通线路]           
2023/02/17 07:38:59 成都联通 119.6.6.6       联通4837[普通线路]           
2023/02/17 07:38:59 成都移动 211.137.96.205  移动CMI [普通线路]           
------------------回程路由--感谢fscarmen开源及PR----------------------
IPv4 ASN: netcup GmbH
IPv6 ASN: netcup GmbH
依次测试电信，联通，移动经过的地区及线路，核心程序来由: ipip.net ，请知悉!
广州电信 58.60.188.222
0.57 ms  AS197540  德国, 巴伐利亚州, 纽伦堡, anexia.com
2.63 ms  AS47147  德国, 巴伐利亚州, 纽伦堡, anexia.com
0.59 ms  AS47147  德国, 巴伐利亚州, 纽伦堡, anexia.com
0.47 ms  AS1299  德国, 巴伐利亚州, 纽伦堡, telia.com
3.86 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
3.96 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
5.19 ms  AS4134  德国, 黑森州, 法兰克福, chinatelecom.com.cn, 电信
192.82 ms  AS4134  中国, 广东, 广州, chinatelecom.com.cn, 电信
209.40 ms  AS4134  中国, 广东, 深圳, chinatelecom.com.cn, 电信
广州联通 210.21.196.6
0.25 ms  AS197540  德国, 巴伐利亚州, 纽伦堡, anexia.com
0.34 ms  AS47147  德国, 巴伐利亚州, 纽伦堡, anexia.com
0.41 ms  AS47147  德国, 巴伐利亚州, 纽伦堡, anexia.com
0.46 ms  AS1299  德国, 巴伐利亚州, 纽伦堡, telia.com
3.62 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
3.67 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
3.57 ms  AS4837  德国, 黑森州, 法兰克福, chinaunicom.com, 联通
166.46 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
167.20 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
155.91 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
161.88 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
160.85 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
广州移动 120.196.165.2
0.32 ms  AS197540  德国, 巴伐利亚州, 纽伦堡, anexia.com
2.96 ms  AS47147  德国, 巴伐利亚州, 纽伦堡, anexia.com
0.54 ms  AS47147  德国, 巴伐利亚州, 纽伦堡, anexia.com
0.48 ms  AS1299  德国, 巴伐利亚州, 纽伦堡, telia.com
3.63 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
3.78 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
4.46 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
4.51 ms  AS58453  德国, 黑森州, 法兰克福, chinamobile.com, 移动
220.71 ms  AS58453  中国, 上海, chinamobile.com, 移动
223.21 ms  AS58453  中国, 广东, 广州, chinamobile.com, 移动
230.88 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
225.40 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
225.12 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
227.67 ms  AS9808  中国, 广东, 广州, chinamobile.com, 移动
235.69 ms  AS56040  中国, 广东, 深圳, chinamobile.com, 移动
229.02 ms  AS56040  中国, 广东, 深圳, chinamobile.com, 移动
--------网络测速--由teddysun和superspeed开源及spiritlhls整理----------
测速点位置       上传速度        下载速度        延迟
Speedtest.net    920.49 Mbps     928.41 Mbps     13.97 ms
洛杉矶           181.92 Mbps     861.00 Mbps     161.57 ms
新加坡           182.19 Mbps     1057.36 Mbps    185.67 ms
中国香港         199.26 Mbps     768.94 Mbps     194.71 ms
电信上海         153.22 Mbps     872.74 Mbps     195.34 ms
联通上海         202.76 Mbps     678.46 Mbps     281.23 ms
联通湖南长沙     223.45 Mbps     371.32 Mbps     171.07 ms
移动广西南宁     262.54 Mbps     740.42 Mbps     207.49 ms
移动宁夏银川     2.12 Mbps       116.77 Mbps     257.41 ms
----------------------------------------------------------------------
 总共花费      : 7 分 16 秒
 时间          : Fr 17. Feb 07:44:35 CET 2023
----------------------------------------------------------------------
```

