---
layout: post
title: "Linux 准备禁用微软的 RNDIS 协议驱动 "
date: 2023-01-16T07:32:30.000Z
author: Solidot
from: https://www.solidot.org/story?sid=73897
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1673854350000-->
[Linux 准备禁用微软的 RNDIS 协议驱动](https://www.solidot.org/story?sid=73897)
------

<div>
出于安全担忧 Linux 准备禁用微软的 RNDIS 协议驱动。RNDIS 代表 Remote Network Driver Interface Specification，是一个私有协议，主要使用 USB 协议作为其下层传输，向上层提供虚拟的以太网连接。 除了 Windows，RNDIS 在跨平台环境中没有广泛使用，由于安全担忧，Linux 内核正寻求将 RNDIS 内核驱动转移到 BROKEN Kconfig 选项，因此它在未来的内核构建中将被禁用。在被标记为 BROKEN 一段时间之后，驱动将可能从上游源码树中删除。内核稳定分支维护者 Greg Kroah-Hartman 称，RNDIS 在设计上就是不安全的，因该协议不可能做到安全，禁用其驱动将防止任何人使用它。<p></p>
</div>
