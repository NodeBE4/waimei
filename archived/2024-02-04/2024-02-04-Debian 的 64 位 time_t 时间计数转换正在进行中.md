---
layout: post
title: "Debian 的 64 位 time_t 时间计数转换正在进行中"
date: 2024-02-04T12:28:19.000Z
author: Solidot
from: https://www.solidot.org/story?sid=77304
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1707049699000-->
[Debian 的 64 位 time_t 时间计数转换正在进行中](https://www.solidot.org/story?sid=77304)
------

<div>
为解决 32 位系统的 2038 年问题，Debian Experimental 开始用 64 位时间计数 time_t 重构软件包。2038 年问题是指类 Unix 系统采用的是 32 位时间计数 time_t，计数从 1970 年开始，到 2038 年 1 月将会溢出。Debian 开发者想要确保下一个版本能在 2038 年之后正常工作。此次 64 位 time_t 转换涉及到逾 1200 个软件包。下一个版本 Debian 13 Trixie 将于 2025 年发布，有充裕的时间完成 2038 年问题的处理。<p></p>
</div>
