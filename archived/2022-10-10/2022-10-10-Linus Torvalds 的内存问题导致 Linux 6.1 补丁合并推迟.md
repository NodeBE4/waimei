---
layout: post
title: "Linus Torvalds 的内存问题导致 Linux 6.1 补丁合并推迟"
date: 2022-10-10T15:48:02.000Z
author: Solidot
from: https://www.solidot.org/story?sid=73011
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1665416882000-->
[Linus Torvalds 的内存问题导致 Linux 6.1 补丁合并推迟](https://www.solidot.org/story?sid=73011)
------

<div>
Linux 6.1 正处于补丁合并阶段，一位内核开发者向  Linus Torvalds 询问是否错过了一个 Git Pull 请求。Linux 作者周日<a href="https://lkml.iu.edu/hypermail/linux/kernel/2210.1/00691.html">证实</a>因为内存问题他现在正以非常慢的速度执行合并队列。Torvalds 的主工作电脑是一台 AMD 线程撕裂者 3970x 工作站，过去几天电脑稳定性出了问题，出现随机的内存损坏错误。他一开始以为是一个新的内核 bug，<a href="https://www.theregister.com/2022/10/10/linus_torvalds_ecc_memory_fail/" target="_blank">检查后发现是内存条问题</a>。他订购了新的 ECC 内存条，替换旧内存条。Torvalds 是在新冠疫情早期组装新电脑的，当时 ECC 内存条稀缺且昂贵，他为此还公开抱怨了英特尔的营销手段，宣称 ECC 内存是为服务器和嵌入式设备服务的，导致一般用户难以购买到便宜的 ECC 内存条。
</div>
