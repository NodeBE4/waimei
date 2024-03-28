---
layout: post
title: "Tor 项目推出模拟 HTTPS 流量的新网桥 WebTunnel"
date: 2024-03-13T13:24:07.000Z
author: Solidot
from: https://www.solidot.org/story?sid=77586
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1710336247000-->
[Tor 项目推出模拟 HTTPS 流量的新网桥 WebTunnel](https://www.solidot.org/story?sid=77586)
------

<div>
Tor 项目正式推出了模拟 HTTPS 流量的新网桥 WebTunnel。网桥是不公开的 Tor 中继。WebTunnel 通过模拟  HTTPS 流量增加屏蔽 Tor 连接的难度。审查者不可能完全屏蔽 HTTPS 连接，因为这会导致绝大部分服务无法访问。Tor 项目称，WebTunnel 的工作原理是将负载（Payload）连接包装成类 WebSocket HTTPS 连接，在网络观察者眼里就像普通的 HTTPS (WebSocket) 连接。使用 WebTunnel 网桥需要用户去获取相关网桥地址，手动添加到 Tor 浏览器中。WebTunnel 网桥数量还不多，目前无法在伊朗部分地区使用，在其它国家能正常工作。<p></p>
</div>
