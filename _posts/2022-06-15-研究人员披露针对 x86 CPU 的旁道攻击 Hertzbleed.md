---
layout: post
title: "研究人员披露针对 x86 CPU 的旁道攻击 Hertzbleed"
date: 2022-06-15T06:11:07.000Z
author: Solidot
from: https://www.solidot.org/story?sid=71832
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1655273467000-->
[研究人员披露针对 x86 CPU 的旁道攻击 Hertzbleed](https://www.solidot.org/story?sid=71832)
------

<div>
伊利诺伊香槟（UIUC）、得州奥斯汀（UT Austin）和华盛顿大学的研究人员<a href="https://www.hertzbleed.com/">披露</a>针对 x86 CPU 的新旁道攻击，他们将其命名为 <a href="https://www.hertzbleed.com/hertzbleed.pdf" target="_blank">Hertzbleed</a> 并创建了一个 Logo 以突出其严重性。Hertzbleed 利用了现代 x86 处理器的动态频率调整，CPU 的频率会因为正在处理的数据而存在差异，相同的程序能在不同的 CPU 频率上运行，因此有着不同的实际时间，远程攻击者能观察这一变化并利用它窃取加密密钥。所有英特尔处理器、AMD  Ryzen 处理器都受到该攻击的影响，研究人员去年第三季度就向英特尔报告了漏洞，但应英特尔要求一直到 6 月 14 日才公开漏洞，原因未知。英特尔和 AMD 都没有计划释出微码更新缓解攻击，权宜之计是禁用动态频率调整——英特尔称其为睿频加速技术（Turbo Boost），AMD 称之为精准智能超频(Precision Boost)。
</div>
