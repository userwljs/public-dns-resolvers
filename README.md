# public-dns-resolvers

个人推荐 Cloudflare DNS、AliDNS。

# 中国 DNS 服务器

## 114DNS

[https://www.114dns.com/](https://www.114dns.com/)

比较纯净的 DNS，IPv4，不支持加密。

纯净无劫持: 
首选: `114.114.114.114`
备用: `114.114.115.115`

拦截钓鱼病毒木马网站: 
首选: `114.114.114.119`
备用: `114.114.115.119`

拦截色情网站: 
首选: `114.114.114.110`
备用: `114.114.115.110`

## AliDNS

[https://alidns.com/](https://alidns.com/)

阿里运营的 DNS，IPv4&IPv6，支持加密。

IPv4: 
首选: `223.5.5.5`
备用: `223.6.6.6`

IPv6: 
首选: `2400:3200::1`
备用: `2400:3200:baba::1`

DoH: 
`https://dns.alidns.com/dns-query`

DoT: 
`dns.alidns.com`

DoQ：
`quic://dns.alidns.com:853`

## DNSPod

[https://www.dnspod.cn/Products/publicdns/](https://www.dnspod.cn/Products/publicdns/)

腾讯运营的 DNS，IPv4&IPv6，支持加密。

IPv4: 
`119.29.29.29`

IPv6: 
`2402:4e00::`

DoH: 
`https://doh.pub/dns-query`

DoH（IP）: 
`https://1.12.12.12/dns-query`
`https://120.53.53.53/dns-query`

DoH（国密）: 
`https://sm2.doh.pub/dns-query`

DoT: 
`dot.pub`

DoT（IP）: 
`1.12.12.12`
`120.53.53.53`

## 360 安全 DNS

[https://sdns.360.net/dnsPublic.html/](https://sdns.360.net/dnsPublic.html/)

360 运营的 DNS，IPv4，支持加密。

电信、移动、铁通 IPv4: 
首选: `101.226.4.6`
备用: `218.30.118.6`

联通 IPv4: 
首选: `123.125.81.6`
备用: `140.207.198.6`

DoT: 
`dot.360.cn`

DoH: 
`https://doh.360.cn/dns-query`

## OneDNS

[https://www.onedns.net/personal/](https://www.onedns.net/personal/)

微步在线运营的 DNS，IPv4&IPv6，支持加密。

### OneDNS 拦截版

防护各类恶意软件，过滤广告骚扰。

IPv4: 
首选: `52.80.66.66`
备用: `117.50.11.11`

IPv6: 
首选: `2400:7fc0:849e:200::4`
备用: `2404:c2c0:85d8:901::4`

DoH: 
`https://doh.onedns.net/dns-query`

DoT: 
`dot.onedns.net`

### OneDNS 纯净版

不对访问网站进行任何过滤拦截，直接返回其真实的响应结果。

IPv4: 
首选: `117.50.10.10`
备用: `52.80.52.52`

IPv6: 
首选: `2400:7fc0:849e:200::8`
备用: `2404:c2c0:85d8:901::8`

DoH: 
`https://doh-pure.onedns.net/dns-query`

DoT: 
`dot-pure.onedns.net`

### OneDNS 家庭版

防护各类恶意软件，过滤广告骚扰。

IPv4: 
首选: `117.50.60.30`
备用: `52.80.60.30`

## 关胜云去广告 DNS

[https://dns.dns1.top/](https://dns.dns1.top/)

使用 AdGuardHome 搭建的私人 DNS，上游 DNS 未知，支持加密。域名更换频繁，如果发现用不了请提 issue。

DoT: 
`2024.dns1.top`
`tls://2024.dns1.top:853`

DoH: 
`https://2024.dns1.top/dns-query/`

DoQ: 
`quic://2024.dns1.top:853`

# 国外 DNS 服务器

## Google Public DNS

[https://developers.google.cn/speed/public-dns](https://developers.google.cn/speed/public-dns)

由 Google 运营，免费的全球 DNS 解析服务，支持加密。

IPv4: 
首选: `8.8.8.8`
备用: `8.8.4.4`

IPv6: 
首选: `2001:4860:4860::8888`
备选: `2001:4860:4860::8844`

DoH: 
`https://dns.google/dns-query`

## Google Public DNS64

[https://developers.google.cn/speed/public-dns/docs/dns64](https://developers.google.cn/speed/public-dns/docs/dns64)

由 Google 运营，免费的全球 DNS 解析服务，仅支持 IPv6，支持加密。

IPv6: 
首选: `2001:4860:4860::6464`
备选: `2001:4860:4860::64`

DoH: 
`https://dns64.dns.google/dns-query`

DoT: 
`dns64.dns.google`

## Cloudflare DNS

[https://developers.cloudflare.com/1.1.1.1/setup/](https://developers.cloudflare.com/1.1.1.1/setup/)

1.1.1.1 是 Cloudflare 的公共 DNS 解析器。它提供了一种快速且私密的方式来浏览互联网。

### Cloudflare DNS 无修改

原汁原味的 DNS。

IPv4: 
首选: `1.1.1.1`
备选: `1.0.0.1`

IPv6: 
首选: `2606:4700:4700::1111`
备选: `2606:4700:4700::1001`

DoH: `https://cloudflare-dns.com/dns-query`

DoT: `one.one.one.one`

### Cloudflare DNS 阻止恶意软件

阻止恶意软件。

IPv4: 
首选: `1.1.1.2`
备选: `1.0.0.2`

IPv6: 
首选: `2606:4700:4700::1112`
备选: `2606:4700:4700::1002`

DoH: `https://security.cloudflare-dns.com/dns-query`

DoT: `security.cloudflare-dns.com`

### Cloudflare DNS 阻止恶意软件和成人内容。

阻止恶意软件和成人内容。

IPv4: 
首选: `1.1.1.3`
备选: `1.0.0.3`

IPv6: 
首选: `2606:4700:4700::1113`
备选: `2606:4700:4700::1003`

DoH: `https://family.cloudflare-dns.com/dns-query`

DoT: `family.cloudflare-dns.com`

## AdGuard Public DNS

[https://adguard-dns.io/zh_cn/public-dns.html](https://adguard-dns.io/zh_cn/public-dns.html)

**这不是客制化的 AdGuard DNS**。

### AdGuard DNS 默认服务器

AdGuard DNS 拦截广告和跟踪器。

IPv4: 
首选: `94.140.14.14`
备选: `94.140.15.15`

IPv6: 
首选: `2a10:50c0::ad1:ff`
备选: `2a10:50c0::ad2:ff`

DoH: `https://dns.adguard-dns.com/dns-query`

DoT: `tls://dns.adguard-dns.com`

DoQ: `quic://dns.adguard-dns.com`

DNSCrypt: `sdns://AQMAAAAAAAAAETk0LjE0MC4xNC4xNDo1NDQzINErR_JS3PLCu_iZEIbq95zkSV2LFsigxDIuUso_OQhzIjIuZG5zY3J5cHQuZGVmYXVsdC5uczEuYWRndWFyZC5jb20`

### AdGuard DNS 无过滤服务器

AdGuard DNS 不拦截广告、跟踪器或其他任何 DNS 请求。

IPv4: 
首选: `94.140.14.140`
备选: `94.140.14.141`

IPv6: 
首选: `2a10:50c0::1:ff`
备选: `2a10:50c0::2:ff`

DoH: `https://unfiltered.adguard-dns.com/dns-query`

DoT: `tls://unfiltered.adguard-dns.com`

DoQ: `quic://unfiltered.adguard-dns.com`

DNSCrypt: `sdns://AQMAAAAAAAAAEjk0LjE0MC4xNC4xNDA6NTQ0MyC16ETWuDo-PhJo62gfvqcN48X6aNvWiBQdvy7AZrLa-iUyLmRuc2NyeXB0LnVuZmlsdGVyZWQubnMxLmFkZ3VhcmQuY29t`

### AdGuard DNS 家庭保护服务器

AdGuard DNS 拦截广告、跟踪器、成人内容，并在可能的情况下启用安全搜索和安全模式。

IPv4: 
首选: `94.140.14.15`
备选: `94.140.15.16`

IPv6: 
首选: `2a10:50c0::bad1:ff`
备选: `2a10:50c0::bad2:ff`

DoH: `https://family.adguard-dns.com/dns-query`

DoT: `tls://family.adguard-dns.com`

DoQ: `quic://family.adguard-dns.com`

DNSCrypt: `sdns://AQMAAAAAAAAAETk0LjE0MC4xNC4xNTo1NDQzILgxXdexS27jIKRw3C7Wsao5jMnlhvhdRUXWuMm1AFq6ITIuZG5zY3J5cHQuZmFtaWx5Lm5zMS5hZGd1YXJkLmNvbQ`
