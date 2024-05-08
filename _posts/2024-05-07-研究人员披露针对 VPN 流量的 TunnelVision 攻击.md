---
layout: post
title: "研究人员披露针对 VPN 流量的 TunnelVision 攻击"
date: 2024-05-07T15:13:13.000Z
author: Solidot
from: https://www.solidot.org/story?sid=78100
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1715094793000-->
[研究人员披露针对 VPN 流量的 TunnelVision 攻击](https://www.solidot.org/story?sid=78100)
------

<div>
研究人员发现了迫使 VPN 应用将流量路由到加密通道之外的新型攻击，该攻击被称为 TunnelVision，影响几乎所有运行在非 Linux 和非 Android 系统上的 VPN。漏洞据信自 2002 年以来就存在并被发现和利用。攻击者能读取、丢弃或修改泄露的流量，而受害者则继续保持 VPN 和互联网的连接。攻击通过操纵分配 IP 地址给本地网络设备的 DHCP 服务器实现。被称为选项 121 的设置允许 DHCP 服务器覆盖默认路由规则，通过使用选项 121 路由 VPN 流量经过 DHCP 服务器，攻击会将数据传送到 DHCP 服务器。攻击允许部分或全部流量路由通过非加密通道，而 VPN 应用仍然会报告流量被加密。Android 系统完全不受影响的原因是它没有实现选项 121。<p></p>
</div>
