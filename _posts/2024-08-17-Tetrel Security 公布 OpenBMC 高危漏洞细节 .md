---
layout: post
title: "Tetrel Security 公布 OpenBMC 高危漏洞细节 "
date: 2024-08-17T13:34:56.000Z
author: Solidot
from: https://www.solidot.org/story?sid=79004
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1723901696000-->
[Tetrel Security 公布 OpenBMC 高危漏洞细节](https://www.solidot.org/story?sid=79004)
------

<div>
Shawn the R0ck 写道：“Tetrel Security 公开了一个 SLPD-Lite 漏洞（CVE-2024-41660）的细节，slpd-lite 是 OpenBMC 的组件之一，此漏洞因为由 OpenBMC（部分OEM厂商实现）网络安全产生了严重的影响，因为它允许攻击者在易受攻击的系统上远程执行任意代码。<br>OpenBMC 是一个为服务器开发标准基板管理控制器（BMC）的标准实现框架。BMC允许对服务器硬件进行远程管理，广泛部署在服务器硬件中，提供监控、日志记录功能以及带外恢复和维护工具。由于BMC通常具有高度特权，因此将BMC网络接口隔离到一个独立的管理网络是安全最佳实践。<br>Tetrel在审查OpenBMC源代码时发现了slpd-lite子组件中的两个内存损坏漏洞。在典型部署中，成功利用这些漏洞将允许具有对BMC管理网络访问权限的攻击者完全攻陷BMC。<br>第一个漏洞涉及堆中分配的数据的越界读取，可能泄露信息给攻击者。第二个漏洞允许攻击者在堆中分配的数据结构范围之外进行写入。结合这两个漏洞，可以直接实现远程漏洞利用。Tetrel公开了漏洞成因，和相关技术细节，包括代码片段和漏洞的潜在利用方式。同时，还提供了有关如何确认堆损坏可能性的重现步骤，以及在Ubuntu 22.04.04 LTS上测试漏洞的过程。<br>如果你的数据中心使用了集成spld-lite的OEM厂商提供的BMC（无论是否基于OpenBMC)，务必尽快升级。HardenedVault的OpenBMC实现由于spld-lite并没有集成，所以不受影响。”<p></p>
</div>
