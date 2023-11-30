---
layout: post
title: "英特尔修复高危 CPU 漏洞 Reptar"
date: 2023-11-15T10:38:09.000Z
author: Solidot
from: https://www.solidot.org/story?sid=76627
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1700044689000-->
[英特尔修复高危 CPU 漏洞 Reptar](https://www.solidot.org/story?sid=76627)
------

<div>
英特尔周二推送了微码更新，修复高危 CPU 漏洞 Reptar（CVE-2023-23583）。该漏洞影响几乎所有现代英特尔处理器，可被用于攻击云端主机。Reptar 与 CPU 管理前缀有关，Intel x64 解码通常允许忽略冗余前缀而不会有任何后果，但 Google 安全研究员 Tavis Ormandy 在测试时发现，在支持“快速短重复移动（fast short repeat move）”的英特尔处理器上运行 REX 前缀会产生“意料之外的结果”。一旦触发，可能导致虚拟机中的  guest 账号执行不信任代码而导致系统崩溃，或者可用于提权。<p></p>
</div>
