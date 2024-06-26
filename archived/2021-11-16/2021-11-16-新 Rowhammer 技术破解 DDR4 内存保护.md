---
layout: post
title: "新 Rowhammer 技术破解 DDR4 内存保护"
date: 2021-11-16T12:05:37.000Z
author: Solidot
from: https://www.solidot.org/story?sid=69637
tags: [ Solidot ]
categories: [ Solidot ]
---
<!--1637064337000-->
[新 Rowhammer 技术破解 DDR4 内存保护](https://www.solidot.org/story?sid=69637)
------

<div>
Rowhammer 漏洞利用允许非特权攻击者修改或破坏存储在易受攻击内存芯片中的数据，制造商后来为内存芯片加入抵御此类攻击的保护措施，<a href="https://arstechnica.com/gadgets/2021/11/ddr4-memory-is-even-more-susceptible-to-rowhammer-attacks-than-anyone-thought/#p3">但最新方法瓦解了保护</a>，事实上所有 DDR4 模块都易受 Rowhammer 攻击。<br><br>Rowhammer 攻击工作原理是每秒数百万次访问或锤击易受攻击的芯片内的物理行，导致相邻行中的比特翻转，意味着 1 变为 0，反之亦然。研究人员证明，这些攻击可被用于为不受信任的应用程序提供几乎不受限制的系统权限，绕过防止恶意代码访问敏感操作系统资源的安全沙箱，Root 或者感染 Android 设备等。<br><br>之前所有的 Rowhammer 攻击都以相同的模式敲击行，例如单面、双面或n面。在所有三种情况下，这些“攻击者”行——导致附近“受害”行比特翻转的那些行——被访问的次数相同。周一发表的<a href="https://comsec.ethz.ch/research/dram/blacksmith/">研究</a>提出一种新 Rowhammer 技术。它使用非均匀模式以不同的频率访问两个或多个攻击者行。结果测试池中所有 40 个随机挑选的 DIMM 都出现比特翻转，成功率高于之前的测试，之前在 42 块芯片中只有 13 块出现比特翻转。研究作者 Kaveh Razavi 和 Patrick Jattke 在一封电邮中写道：“我们发现，通过创建特殊的内存访问模式，可绕过部署在 DRAM 中所有的防御措施。根据分析，这将可能被已知攻击入侵的设备比例增加到 80%。由于硬件特性，这些问题无法修复，将在未来很多年中继续存在。”<br><br>非均匀模式对目标行刷新也有效。这种缩写为 TRR 的防御措施因供应商而异，但是通常会跟踪行被访问的次数，在出现滥用迹象时为相邻的受害行补电。防御的失效给芯片制造商带来了进一步的压力，推动他们想方设法抵御此类攻击——很多人原本认为较新类型的存储芯片可以抵御它了。
</div>
