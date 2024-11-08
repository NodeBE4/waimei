---
layout: post
title: "俄罗斯屏蔽 Cloudflare 的 ECH 连接"
date: 2024-11-08T03:44:24.000Z
author: Solidot
from: https://www.solidot.org/story?sid=79714
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1731037464000-->
[俄罗斯屏蔽 Cloudflare 的 ECH 连接](https://www.solidot.org/story?sid=79714)
------

<div>
Gundaz Aghayev 写道：Cloudflare 最近部署的隐私保护协议 Encrypted Client Hello(ECH)不小心规避了各国的审查系统，俄罗斯已将其封锁。封锁只针对 Cloudflare，其他 ECH 不受影响，俄国 DPI 系统 TSPU (техническиесредства противодействия угрозам) 目前的检测条件是包含 `cloudflare-ech.com`的 TLS SNI 扩展和 TLS ECH 扩展，缺一不可。俄罗斯政府机构“互联网监控和控制中心” (ЦМУ ССОП) 发表文章建议禁用非法的 TLS ECH 技术，甚至停止使用 Cloudflare CDN，转而使用俄国国内的替代如“国家 DDoS 攻击应对系统” (НСПА)。它还指控 Cloudflare 公司由美国国务院授意、侵害各国信息主权。<p></p>
</div>
