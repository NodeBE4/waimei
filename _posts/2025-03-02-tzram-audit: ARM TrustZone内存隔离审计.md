---
layout: post
title: "tzram-audit: ARM TrustZone内存隔离审计"
date: 2025-03-02T15:38:58.000Z
author: Solidot
from: https://www.solidot.org/story?sid=80694
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1740929938000-->
[tzram-audit: ARM TrustZone内存隔离审计](https://www.solidot.org/story?sid=80694)
------

<div>
Shawn C  写道:<i>ARM TrustZone 的设计初衷是将内存划分为两个世界：非安全世界（运行丰富执行环境，如 Linux/Android）和安全世界（运行受信任的执行环境，即 TEE OS）。它已在汽车、移动设备和硬件钱包等行业广泛部署。关键点如下：<br>* Linux 内核运行在非安全 EL1（NS.EL1）。<br>* TEE OS 运行在安全 EL1（S.EL1）。<br>* 安全监控器（例如 ARM Trusted Firmware，ATF）运行在安全 EL3（S.EL3）。<br>* Linux 内核通过发出 SMC（安全监控调用）指令给安全监控器，后者再将请求路由至 TEE OS。<br>* 默认情况下，ARM 核心架构没有为 MMU 提供安全扩展。这意味着，如果 SoC 供应商没有集成专用的 TZASC（TrustZone 地址空间控制器）IP，则两个世界之间的内存隔离将无法有效实现。<br>* 任何需要安全处理的外设必须由安全世界管理。因此，SoC 必须集成额外的 IP 用于 TZPC（TrustZone 防护控制器）。这一方法与 x86_64 生态系统中使用的 MMU、IOMMU、EPC、SGX 或 TDX 有显著不同。<br>* ARM 参考模型允许安全世界和非安全世界使用相同的物理地址（例如，非安全物理地址 np:0x1000 与安全物理地址 sp:0x1000）对应内存系统中不同的位置。然而，大多数 SoC 供应商倾向于避免这种复杂性（即 np:0x1000 和 sp:0x1000 指的是相同位置）。<br>* 与 x86 相比，ARM 的 TEE 更类似于系统管理模式（SMM）。</i><p></p>
</div>
