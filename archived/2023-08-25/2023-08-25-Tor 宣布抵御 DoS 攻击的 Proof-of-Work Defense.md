---
layout: post
title: "Tor 宣布抵御 DoS 攻击的 Proof-of-Work Defense"
date: 2023-08-25T11:10:17.000Z
author: Solidot
from: https://www.solidot.org/story?sid=75895
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1692961817000-->
[Tor 宣布抵御 DoS 攻击的 Proof-of-Work Defense](https://www.solidot.org/story?sid=75895)
------

<div>
Tor 项目宣布了设计抵御 DoS 攻击的工作量防御机制（Proof-of-Work Defense）。工作量证明 PoW 是一种动态的反应机制，在正常工作条件下保持休眠。当 onion 服务面临压力时，PoW 将提示传入的客户端连接连续执行复杂操作，onion 服务将根据客户端的工作量水平进行连接优先排序。此举旨在将 DoS 攻击的成本增加到难以维持的水平，优先考虑合法流量，抑制攻击流量。onion 服务因为优先考虑客户的隐私混淆 IP 地址而容易遭到  DoS 攻击，传统的基于 IP 的速率限制无效，因此 Tor 项目设计了一种工作量证明机制，在不影响客户隐私的同时遏制 DoS 攻击。如果攻击者向 onion 服务发送大量连接请求，PoW 防御会启动增加访问 .onion 网站所需的计算量。增加的计算量对绝大部分设备是可控的，所耗费时间从 5 毫秒到 30 毫秒。攻击流量增加，工作量就会增加，最多需要 1 分钟的工作量。整个过程对用户是不可见的。<p></p>
</div>
