---
layout: post
title: "对 AMD Zen 系列平台的 RowHammer 比特翻转攻击"
date: 2024-03-26T15:10:27.000Z
author: Solidot
from: https://www.solidot.org/story?sid=77702
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1711465827000-->
[对 AMD Zen 系列平台的 RowHammer 比特翻转攻击](https://www.solidot.org/story?sid=77702)
------

<div>
研究人员披露了针对 AMD Zen 2 和 Zen 3 平台的 RowHammer 比特翻转攻击 ZenHammer。RowHammer 攻击指的是应用反复访问 DDR 内存芯片的特定区域导致比特翻转。比特翻转（Bitflips）是指储存在电子设备上的个别比特发生翻转的事件，比如从 0 变为 1 或反之亦然。研究人员表示，尽管部署了缓解措施，他们仍然能针对 Zen 2 和 Zen 3 系统上的 DDR4 触发 Rowhammer 比特翻转。研究人员还使用 ZenHammer 攻击首次演示了对 DDR5 的  RowHammer 比特翻转。研究人员认为 Error Correction Codes(ECC)内存无法提供对 RowHammer 攻击的完整防御，只是增加了利用难度。研究人员在 2024 年 2 月 26 日通知了 AMD，应其要求到 2024 年 3 月 25 日才公开披露该漏洞。<p></p>
</div>
