# public-dns-resolvers

# 中国 DNS 服务器

## 114DNS

[https://www.114dns.com/](https://www.114dns.com/)

比较纯净的 DNS，IPv4，不支持加密。

纯净无劫持：
首选：`114.114.114.114`
备用：`114.114.115.115`

拦截钓鱼病毒木马网站：
首选：`114.114.114.119`
备用：`114.114.115.119`

拦截色情网站：
首选：`114.114.114.110`
备用：`114.114.115.110`

## AliDNS

[https://alidns.com/](https://alidns.com/)

阿里运营的 DNS，IPv4&IPv6，支持加密。

IPv4：
首选：`223.5.5.5`
备用：`223.6.6.6`

IPv6：
首选：`2400:3200::1`
备用：`2400:3200:baba::1`

DoH：
`https://dns.alidns.com/dns-query`

DoT：
`dns.alidns.com`

## DNSPod

[https://www.dnspod.cn/Products/publicdns/](https://www.dnspod.cn/Products/publicdns/)

腾讯运营的 DNS，IPv4&IPv6，支持加密。

IPv4：
`119.29.29.29`

IPv6：
`2402:4e00::`

DoH：
`https://doh.pub/dns-query`

DoH（IP）：
`https://1.12.12.12/dns-query`
`https://120.53.53.53/dns-query`

DoH（国密）：
`https://sm2.doh.pub/dns-query`

DoT：
`dot.pub`

DoT（IP）：
`1.12.12.12`
`120.53.53.53`

## 360 安全 DNS

[https://sdns.360.net/dnsPublic.html/](https://sdns.360.net/dnsPublic.html/)

360 运营的 DNS，IPv4，支持加密。

电信、移动、铁通 IPv4：
首选：`101.226.4.6`
备用：`218.30.118.6`

联通 IPv4：
首选：`123.125.81.6`
备用：`140.207.198.6`

DoT：
`dot.360.cn`

DoH：
`https://doh.360.cn/dns-query`

## OneDNS

[https://www.onedns.net/personal/](https://www.onedns.net/personal/)

微步在线运营的 DNS，IPv4&IPv6，不支持加密。

拦截版 IPv4：
首选：`52.80.66.66`
备用：`117.50.11.11`

拦截版 IPv6：
首选：`2400:7fc0:849e:200::4`
备用：`2404:c2c0:85d8:901::4`

纯净版 IPv4：
首选：`117.50.10.10`
备用：`52.80.52.52`

纯净版 IPv6：
首选：`2400:7fc0:849e:200::8`
备用：`2404:c2c0:85d8:901::8`

家庭版 IPv4：
首选：`117.50.60.30`
备用：`52.80.60.30`

## 关胜云去广告 DNS

[https://dns.dns1.top/](https://dns.dns1.top/)

不是广告（-w-），使用 AdGuardHome 搭建的私人 DNS，上游 DNS 未知，支持加密。域名更换频繁，如果发现用不了请提 issue。

DoT：
`2024.dns1.top`
`tls://a.newlover.cn:853`

DoH：
`https://a.newlover.cn/dns-query/a`

DoQ：
`quic://a.newlover.cn:853`
