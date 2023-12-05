## 前言

前段时间用 ACME 申请证书的时候，不知道为什么，莫名其妙没有自动删除 TXT 记录，导致我的域名里面有几百条 TXT 记录。

这里就推荐一个方法，可以批量删除 Cloudflare 的 DNS 记录。

## 推荐阅读

[acne.sh  一键申请可自动续期的 SSL 证书 | GAKIYUKR'S Blog](https://www.gakiyukr.net/archives/314)

## 优劣势

1. 可以批量删除 DNS 记录
2. 只能一口气删掉所有 DNS 记录
3. 官方的一键导入导出无法记录 CDN 是否开启，需要后续手动开启。

## 脚本代码

本脚本来源于 Cloudflare 社区

[Bulk delete DNS records? - Developers / API - Cloudflare Community](https://community.cloudflare.com/t/bulk-delete-dns-records/421686)

```
$API_TOKEN = "<API TOKEN>"
$ZONE_ID   = "<ZONE ID>"

$baseUrl = "https://api.cloudflare.com/client/v4/zones/$ZONE_ID/dns_records"

$headers = @{
  'Authorization' = "Bearer $API_TOKEN"
  'Content-Type'  = "application/json"
}

$listUrl = $baseUrl + '?per_page=500'
Write-Host $listUrl
$records = Invoke-RestMethod -Uri $listUrl -Method 'GET' -Headers $headers
$records = $records | Select-Object -ExpandProperty result

foreach ($record in $records) {
  Write-Host "Deleting $($record.name) that points to $($record.content)"

  $deleteUrl = $baseUrl + '/' + $record.id
  Invoke-RestMethod -Uri $deleteUrl -Method 'DELETE' -Headers $headers
  Write-Host $deleteUrl
}
```

Zone ID 在此处获取：

![](https://s3-jp-ap-3.040407.xyz/oss/photos/msedge_tdZHDPogv7.png)

Api Token 需要自行创建：

![](https://s3-jp-ap-3.040407.xyz/oss/photos/msedge_YGsxUSt5AX.png)

使用默认模板即可，不放心的话可以指定该 Token 的权限

![](https://s3-jp-ap-3.040407.xyz/oss/photos/msedge_HFmvNnCIsQ.png)

​	记得提前去导出 DNS 记录，编辑导出的 TXT 文件，删除你不想要的记录即可。

![](https://s3-jp-ap-3.040407.xyz/oss/photos/msedge_hT3feYFusQ.png)

运行脚本，删除完毕后再将刚刚编辑好的记录导入回去即可。