# 网络现状

中国科学院（CAS）使用的是中国科技网（CSTNET）[1][1] [2][2]，中国科学院大学（UCAS）使用的是中国教育网（CERNET）[1][3]。

注：国内 ISP 的 ASN 可在[这里][4]查询。  

## 网络带宽

- 雁栖湖校区宿舍网口IPv6可能为千兆上下行对等
- TODO

## 网址分配

- UCAS 中关村宿舍楼分配的 IPv6 使用 DHCPv6，无 PD 前缀。
- UCAS 雁栖湖宿舍楼墙口和无线网分配的 IPv6 使用 DHCPv6，无 PD 前缀；分配的 IPv4 为公网 IP，暂未发现防火墙（如屏蔽 80 端口的情况）。
- UCAS 雁栖湖教学楼、学园楼、图书馆的无线网有一定概率分配到 IPv6 地址。分配的 IPv4 都在 `10.0.0.0/8` 下，不同位置的具体网段不同，每个子网为 `/23` 大小。无需认证登录即可连通宿舍楼的 IP。
- UCAS 雁栖湖西区宿舍可连到联通热点 `ChinaUnicom`，免费，但是需要手动申请开通，登录后分配到公网 IPv4 地址，暂未发现防火墙。
- ISCAS 分配的 IPv6 使用 DHCPv6，无 PD 前缀。
- //待补充

在 UCAS 中关村宿舍 F 座得到的 IP 在 `2001:cc0:2020:3020::/64` 子网下，且主机地址是根据网卡 MAC 生成的 EUI-64 IID。

注：在 ISCAS，因为各实验室自行管理内网，不是所有实验室都支持 IPv6。  

[1]: https://ipinfo.io/AS17965
[2]: https://ipinfo.io/AS37944
[3]: https://ipinfo.io/AS4538
[4]: https://ipinfo.io/countries/cn
