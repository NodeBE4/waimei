---
layout: post
title: "Cloudflare 称其下一代服务器不使用英特尔 CPU"
date: 2021-09-02T04:54:22.000Z
author: Solidot
from: https://www.solidot.org/story?sid=68781
tags: [ Solidot ]
categories: [ Solidot ]
---
<!--1630558462000-->
[Cloudflare 称其下一代服务器不使用英特尔 CPU](https://www.solidot.org/story?sid=68781)
------

<div>
CDN 服务商 Cloudflare 透露，考虑到功耗过高的问题，<a href="https://www.theregister.com/2021/09/01/cloudflare_picks_amd_again/" target="_blank">他们不打算在下一代自制服务器内使用英特尔芯片</a>。平台运营工程师 Chris Howells 在本周二发表的<a href="https://blog.cloudflare.com/the-epyc-journey-continues-to-milan-in-cloudflares-11th-generation-edge-server/">官方博文</a>中提到，自 2020 年年中以来，Cloudflare 就一直在努力设计其第 11 代服务器。Howells 写道，“我们评估了英特尔最新一代 Ice Lake 至强处理器。虽然英特尔芯片在原始性能上与 AMD 不相伯仲，但每台服务器的功耗会高出数百瓦——规模化场景下的差异将极为巨大。”Cloudflare 的评估报告表明，他们将在全球 200 多个边缘站点服务器上采用 AMD 的 64 核 Epyc 7713 处理器。另外能耗考量也让他们将最初的三块磁盘设计调整为两块磁盘。他们决定用两块 1.92 TB 的三星硬盘取代初始设计中的三块 960 GB 单元，这不仅能让存储容量额外增加 1TB，同时也令功耗降低 6 瓦。Howells 还提到，测试数据表明在将现有 384 GB 内存升级至 512 GB 之后，并没有产生显著的性能提升——因此可以证明 384 GB 已完全够用。但有必要将内存从 DDR4-2933 升级为 DDR4-3200，以略有增加的成本换取合理的性能提升。
</div>
