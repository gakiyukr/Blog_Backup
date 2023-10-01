演示系统为Debian（应该是都通用，起码和Ubuntu通用）机器本身有150g系统盘，附加了500g硬盘。

首先使用硬件测试脚本，看一下机器现有的储存空间。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-22_09-17-42.png)

输入 ```lsblk``` 查看所有储存设备挂载情况。可以看到，名叫sda的分区就是我们需要挂载的（至于为什么不是整500g？这就想u盘厂商是 1000M=1G，Windows却是1024M=1G）

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-22_09-30-39.png)

然后添加新的硬盘分区，使用```fdisk /dev/分区名```。

输入n创建新分区。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-22_09-43-54.png)

输入p创建主分区

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-22_09-44-55.png)

输入1，后面两步步直接回车

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-22_09-46-06.png)

然后输入w保存退出。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-22_09-48-23.png)

接下来格式化分区，使用`mkfs -t ext4 /dev/分区名` 命令

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-22_09-50-07.png)

接下来挂载分区，使用` mount /dev/分区名 /指定挂载的路径`

（该目录要提前创建，并且保持为空）



然后就可以再次使用一下配置检测脚本，看一下硬盘大小了。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_12-22_09-55-25.png)

这个时候可以看到，硬盘已经变大了，挂载成功。

（如果你作为储存使用，记得要把文件存进挂载的目录，存到其他地方还是占用系统盘空间）