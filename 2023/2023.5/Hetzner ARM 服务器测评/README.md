## 前言

德国老牌服务商 Hetzner 近期上线了 ARM 架构的 VPS ，这里有一篇[官方公告](https://www.hetzner.com/presse-berichte/2022/03/167137)。

ARM 一般在白嫖 Oracle 时比较常见，平常还真没怎么见过卖 ARM 的商家。

价格上还算亲民，CAX11（AMD 下的 CX21）只需要 3.79 EUR/月。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_05-02_12-24-46.png)

但是 ARM 平台上还是有很多东西没法用，或者是有莫名其妙的 BUG，并不好用。

生产环境还是不建议用 ARM 平台。

## 详细配置

```
测评频道: https://t.me/vps_reviews                    
版本：2023.04.29
更新日志：融合怪十代目(集合百家之长)(专为测评频道小鸡而生)
-----------------感谢teddysun和superbench和yabs开源-------------------
 CPU 型号          : Neoverse-N1
 CPU 核心数        : 2
 硬盘空间          : 38.2 GB (1.3 GB 已用)
 内存              : 3829 MB (73 MB 已用)
 Swap              : 0 MB (0 MB 已用)
 系统在线时间      : 0 days, 0 hour 8 min
 负载              : 0.19, 0.05, 0.02
 系统              : Debian GNU/Linux 11 (bullseye)
 AES-NI指令集      : ✔ Enabled
 VM-x/AMD-V支持    : ❌ Disabled
 架构              : aarch64 (64 Bit)
 内核              : 5.10.0-21-arm64
 TCP加速方式       : cubic
 虚拟化架构        : kvm
 ASN组织           : AS24940 Hetzner Online GmbH
 位置              : Gunzenhausen / DE
 地区              : Bavaria
-------------------CPU测试--感谢lemonbench开源------------------------
 -> CPU 测试中 (Fast Mode, 1-Pass @ 5sec)
 1 线程测试(1核)得分: 		3398 Scores
 2 线程测试(多核)得分: 		6933 Scores
-------------------内存测试--感谢lemonbench开源-----------------------
 -> 内存测试 Test (Fast Mode, 1-Pass @ 5sec)
 单线程读测试:		30428.35 MB/s
 单线程写测试:		14157.80 MB/s
----------------磁盘IO读写测试--感谢lemonbench开源--------------------
 -> 磁盘IO测试中 (4K Block/1M Block, Direct Mode)
 测试操作		写速度					读速度
 100MB-4K Block		->
 100MB-4K Block		42.9 MB/s (0.10K IOPS, 2.44s)		->
 100MB-4K Block		42.9 MB/s (0.10 IOPS, 2.44s)		61.4 MB/s (14991 IOPS, 1.71s)
 1GB-1M Block		->
 1GB-1M Block		1.0 GB/s (983 IOPS, 1.02s)		->
 1GB-1M Block		1.0 GB/s (983 IOPS, 1.02s)		1.8 GB/s (1740 IOPS, 0.57s)
-------------------磁盘IO读写测试--感谢yabs开源-----------------------
ARM compatibility is considered *experimental*
  ------   | ---            ----  | ----           ---- 
Read       | 146.70 MB/s  (36.6k) | 1.45 GB/s    (22.8k)
Write      | 146.60 MB/s  (36.6k) | 1.50 GB/s    (23.4k)
Total      | 293.30 MB/s  (73.3k) | 2.96 GB/s    (46.2k)           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 1.76 GB/s     (3.4k) | 1.72 GB/s     (1.6k)
Write      | 1.91 GB/s     (3.7k) | 1.92 GB/s     (1.8k)
Total      | 3.67 GB/s     (7.1k) | 3.65 GB/s     (3.5k)
--------------------流媒体解锁--感谢sjlleo开源------------------------
以下测试的解锁地区是准确的，但是不是完整解锁的判断可能有误，这方面仅作参考使用
----------------Youtube----------------
[IPv4]
连接方式: Youtube Video Server
视频缓存节点地域: 德国法兰克福(FRA15S37)
Youtube识别地域: 无信息(null)
[IPv6]
连接方式: Youtube Video Server
视频缓存节点地域: 德国法兰克福(FRA16S31)
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
 Dazn:					No
 HotStar:				No
 Disney+:				No
 Netflix:				Originals Only
 YouTube Premium:			Yes (Region: DE)
 Amazon Prime Video:			Yes (Region: DE)
 TVBAnywhere+:				Yes
 iQyi Oversea Region:			DE
 Viu.com:				No
 YouTube CDN:				Frankfurt 
 Netflix Preferred CDN:			Vienna  
 Spotify Registration:			No
 Steam Currency:			EUR
=======================================
 以下为IPV6网络测试，若无IPV6网络则无输出
============[ Multination ]============
 Dazn:					Failed (Network Connection)
 HotStar:				No
 Disney+:				Yes (Region: DE)
 Netflix:				Originals Only
 YouTube Premium:			Yes (Region: DE)
 Amazon Prime Video:			Unsupported
 TVBAnywhere+:				Failed (Network Connection)
 iQyi Oversea Region:			Failed
 Viu.com:				Failed
 YouTube CDN:				Frankfurt 
 Netflix Preferred CDN:			Vienna  
 Spotify Registration:			No
 Steam Currency:			Failed (Network Connection)
=======================================
-------------TikTok解锁--感谢lmc999的源脚本及fscarmen PR--------------
 Tiktok Region:		【DE】
--------OpenAi解锁--感谢missuo的OpenAI-Checker项目本人修改优化--------
[IPv4]
Your IP supports access to OpenAI. Region: DE
[IPv6]
Your IP supports access to OpenAI. Region: DE
-----------------欺诈分数以及IP质量检测--本频道原创-------------------
以下仅作参考，不代表100%准确，如果和实际情况不一致请手动查询多个数据库比对
scamalytics数据库:
  欺诈分数(越低越好)：41
  匿名代理: No
  Tor出口节点: No
  服务器IP: Yes
  公共代理: No
  网络代理: No
  搜索引擎机器人: No
ip234数据库：
  欺诈分数(越低越好)：26
ip-api数据库:
  手机流量: No
  代理服务: No
  数据中心: Yes
abuseipdb数据库-abuse得分：0
IP类型:
  IP2Location数据库: Data Center/Web Hosting/Transit
Google搜索可行性：NO
------以下为IPV6检测------
scamalytics数据库:
  欺诈分数(越低越好)：41
  匿名代理: No
  Tor出口节点: No
  服务器IP: Yes
  公共代理: No
  网络代理: No
  搜索引擎机器人: No
abuseipdb数据库-abuse得分：0
IP类型:
  IP2Location数据库: Data Center/Web Hosting/Transit
-----------------三网回程--感谢zhanghanyun/backtrace开源--------------
2023/04/29 13:45:45 北京电信 219.141.136.12  测试超时
2023/04/29 13:45:45 北京联通 202.106.50.1    联通4837[普通线路]           
2023/04/29 13:45:45 北京移动 221.179.155.161 移动CMI [普通线路]           
2023/04/29 13:45:45 上海电信 202.96.209.133  测试超时
2023/04/29 13:45:45 上海联通 210.22.97.1     联通4837[普通线路]           
2023/04/29 13:45:45 上海移动 211.136.112.200 移动CMI [普通线路]           
2023/04/29 13:45:45 广州电信 58.60.188.222   电信163 [普通线路]           
2023/04/29 13:45:45 广州联通 210.21.196.6    联通4837[普通线路]           
2023/04/29 13:45:45 广州移动 120.196.165.24  移动CMI [普通线路]           
2023/04/29 13:45:45 成都电信 61.139.2.69     电信163 [普通线路]           
2023/04/29 13:45:45 成都联通 119.6.6.6       联通4837[普通线路]           
2023/04/29 13:45:45 成都移动 211.137.96.205  移动CMI [普通线路]           
------------------回程路由--感谢fscarmen开源及PR----------------------
IPv4 ASN: Hetzner Online
IPv6 ASN: Hetzner Online
依次测试电信，联通，移动经过的地区及线路，核心程序来由: ipip.net ，请知悉!
广州电信 58.60.188.222
2.99 ms  *  局域网
0.45 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
1.28 ms  AS24940  德国, 巴伐利亚州, 纽伦堡, hetzner.com
1.26 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
0.86 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
3.00 ms  AS24940  德国, 巴伐利亚州, 纽伦堡, hetzner.com
3.50 ms  AS1299  德国, 巴伐利亚州, 纽伦堡, telia.com
6.58 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
6.24 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
7.79 ms  AS4134  德国, 黑森州, 法兰克福, chinatelecom.com.cn, 电信
269.15 ms  AS4134  中国, 广东, 广州, chinatelecom.com.cn, 电信
271.09 ms  AS4134  中国, 广东, 深圳, chinatelecom.com.cn, 电信
广州联通 210.21.196.6
3.64 ms  *  局域网
0.76 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
1.63 ms  AS24940  德国, 巴伐利亚州, 纽伦堡, hetzner.com
22.05 ms  AS24940  德国, 巴伐利亚州, 纽伦堡, hetzner.com
1.21 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
3.39 ms  AS24940  德国, 巴伐利亚州, 纽伦堡, hetzner.com
3.78 ms  AS1299  德国, 巴伐利亚州, 纽伦堡, telia.com
6.69 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
6.46 ms  AS1299  德国, 黑森州, 法兰克福, telia.com
164.67 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
166.01 ms  AS4837  中国, 广东, 广州, chinaunicom.com, 联通
168.16 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
159.96 ms  AS17623  中国, 广东, 深圳, chinaunicom.com, 联通
广州移动 120.196.165.2
3.51 ms  *  局域网
1.64 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
1.53 ms  AS24940  德国, 巴伐利亚州, 纽伦堡, hetzner.com
1.46 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
1.75 ms  AS24940  德国, 萨克森自由州, 法尔肯施泰因, hetzner.com
5.67 ms  AS24940  德国, 黑森州, 法兰克福, hetzner.com
6.99 ms  *  德国, 黑森州, 法兰克福, de-cix.net
6.21 ms  AS58453  德国, 黑森州, 法兰克福, chinamobile.com, 移动
230.03 ms  AS58453  中国, 上海, chinamobile.com, 移动
232.77 ms  AS9808  中国, 上海, chinamobile.com, 移动
228.14 ms  AS9808  中国, 上海, chinamobile.com, 移动
267.87 ms  AS56040  中国, 广东, 广州, chinamobile.com, 移动
265.45 ms  AS56040  中国, 广东, 深圳, chinamobile.com, 移动
------------------------ ecs-net--本频道独创 -------------------------
位置		 上传速度	 下载速度	 延迟	  丢包率
Speedtest.net	 81.13 Mbps	 60.83 Mbps	 3.52	  0.0%
洛杉矶		 548.97 Mbps	 2648.37 Mbps	 167.56	  0.0%
新加坡		 8.79 Mbps	 2482.43 Mbps	 169.48	  2.7%
联通WuXi	 365.65 Mbps	 3479.84 Mbps	 176.63	  0.3%
联通上海5G	 427.00 Mbps	 3089.26 Mbps	 219.95	  0.0%
电信天津	 1.15 Mbps	 2938.88 Mbps	 249.62	  NULL
移动Chengdu	 4.22 Mbps	 4586.09 Mbps	 175.05	  2.3%
移动陕西5G	 2.07 Mbps	 3678.44 Mbps	 382.97	  21.3%
----------------------------------------------------------------------
 总共花费      : 7 分 17 秒
 时间          : Sab Agd 29  1:51:53 carra UTC 2023
----------------------------------------------------------------------
ID    测速服务器信息       上传/Mbps   下载/Mbps   延迟/ms
3633  电信|上海　　　　　　↑ 32.18     ↓ 1796.18   270.29  
17145 电信|安徽合肥５Ｇ　　↑ 4.05      ↓ 722.45    265.53  
5396  电信|江苏苏州５Ｇ　　↑ 223.72    ↓ 3034.24   225.86  
23844 电信|湖北武汉　　　　↑ 8.71      ↓ 2194.08   274.00  
28225 电信|湖南长沙５Ｇ　　↑ 2.13      ↓ 374.30    277.50  
3973  电信|甘肃兰州　　　　↑ 0.53      ↓ 11.72     329.31  
24447 联通|上海５Ｇ　　　　↑ 152.61    ↓ 2731.64   231.38  
4870  联通|湖南长沙　　　　↑ 192.24    ↓ 994.62    171.00  
25858 移动|北京　　　　　　↑ 149.89    ↓ 3115.20   274.72  
----------------------------------------------------------------------
```

