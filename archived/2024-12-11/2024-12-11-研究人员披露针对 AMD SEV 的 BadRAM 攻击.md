---
layout: post
title: "研究人员披露针对 AMD SEV 的 BadRAM 攻击"
date: 2024-12-11T15:48:42.000Z
author: Solidot
from: https://www.solidot.org/story?sid=80025
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1733932122000-->
[研究人员披露针对 AMD SEV 的 BadRAM 攻击](https://www.solidot.org/story?sid=80025)
------

<div>
如果能物理接触硬件，那么硬件的安全性通常就无法保障了。然而在云计算时代，客户的敏感数据都储存在未知地点的云端，由未知身份的服务器管理员维护。如何防止能物理接触设备的人窃取敏感数据？芯片供应商的回应是加入保护措施，确保在服务器被物理篡改或感染恶意软件的情况下敏感数据不会被窃取。本周二，一个国际研究小组公布了针对 AMD SEV 的 BadRAM 攻击。AMD 的 Secure Encrypted Virtualization (SEV)被用于加密虚拟机内存并将其隔离以保障云计算的隐私和信任。研究人员报告，利用不到 10 美元的设备，他们可以篡改 DRAM 模块上的嵌入式 SPD 芯片，绕过 SEV 保护，包括最新版本的 SEV-SNP。AMD 已经释出了补丁，补丁没有影响性能，只是增加了启动时间。<p></p>
</div>
