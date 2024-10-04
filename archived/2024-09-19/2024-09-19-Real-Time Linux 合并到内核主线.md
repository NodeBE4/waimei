---
layout: post
title: "Real-Time Linux 合并到内核主线"
date: 2024-09-19T06:56:38.000Z
author: Solidot
from: https://www.solidot.org/story?sid=79288
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1726728998000-->
[Real-Time Linux 合并到内核主线](https://www.solidot.org/story?sid=79288)
------

<div>
在长达 20 年之后，Real-Time Linux(PREEMPT_RT)合并到内核主线。从 Linux 6.12 开始，所有发行版都将包含实时 Linux 代码。这意味着 Linux 将开始运行在更多任务关键设备和工业硬件上。实时操作系统对时间限制非常严格，需要确保关键任务在指定时间期限内完成。实时内核代码合并到主线的最后一个障碍是重新设计  print_k 函数。print_k 函数最早是 Linus Torvalds 本人开发用于调试的工具，但程序在调用 print_k 时会产生硬延迟，这对于实时系统是不可接受的。今年初内核社区终于在重设 print_k 上达成了一致。<p></p>
</div>
