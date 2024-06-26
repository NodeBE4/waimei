---
layout: post
title: "Google Android 内核开发转向上游优先策略"
date: 2021-09-23T13:47:50.000Z
author: Solidot
from: https://www.solidot.org/story?sid=69035
tags: [ Solidot ]
categories: [ Solidot ]
---
<!--1632404870000-->
[Google Android 内核开发转向上游优先策略](https://www.solidot.org/story?sid=69035)
------

<div>
Google 的 Android 操作系统曾以包含大量下游补丁而臭名昭著，下游补丁增加了维护的难度和操作系统的碎片化。但最近几年 Google 改变了策略，越来越多的代码递交到了上游，Google 同时逐渐转向使用 Android Generic Kernel Image (GKI)作为其所有产品内核的基础，进一步减少碎片化。展望未来，Google <a href="https://www.phoronix.com/scan.php?page=news_item&amp;px=Android-Linux-Upstream-First">采用了上游优先策略</a>，在将功能引入到 Android 系统前首先将其推到上游的主线内核。 Google 的 Todd Kjos 在 Linux Plumbers Conference (LPC2021)&nbsp; 峰会上讨论了该公司的 GKI 计划，表示随着 Android 12 以及基于 Linux 5.10 的 GKI 镜像，他们已经将碎片化减少到基本消除。在&nbsp; Android 12 GKI 中，绝大部分供应商/OEM 内核功能要么进入上游内核，要么被孤立在供应商模块/钩子中，要么合并到 Android Common Kernel。
</div>
