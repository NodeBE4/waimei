---
layout: post
title: "Goolge 修复正被利用的 Android 内核 0day 漏洞"
date: 2025-02-07T13:26:06.000Z
author: Solidot
from: https://www.solidot.org/story?sid=80496
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1738934766000-->
[Goolge 修复正被利用的 Android 内核 0day 漏洞](https://www.solidot.org/story?sid=80496)
------

<div>
Goolge 本月初释出了两组安全补丁 2025-02-01 和 2025-02-05，修复了 48 个漏洞，其中包括一个 Android 内核 0day 高危漏洞。该漏洞编号 CVE-2024-53104，影响 Linux 内核的 USB Video Class(UVC)驱动，属于越界写入 bug，存在于 uvc_driver.c 的 uvc_parse_format()函数中。该漏洞会导致内存损坏、程序崩溃甚至任意代码执行。攻击者可利用该 bug 提权，可用于安装恶意程序、更改或删除数据，或创建拥有完整管理权限的新帐户。该漏洞已被用于针对性的有限攻击。Android 用户最好立即更新到最新的安全补丁。<p></p>
</div>
