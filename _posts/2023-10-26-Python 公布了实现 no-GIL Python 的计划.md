---
layout: post
title: "Python 公布了实现 no-GIL Python 的计划"
date: 2023-10-26T07:05:06.000Z
author: Solidot
from: https://www.solidot.org/story?sid=76453
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1698303906000-->
[Python 公布了实现 no-GIL Python 的计划](https://www.solidot.org/story?sid=76453)
------

<div>
Python 指导委员会宣布接受 PEP 703（Making the Global Interpreter Lock Optional，让全局解释器锁成为可选），公布了实现 no-GIL（或称为自由线程）Python 详细的路线图。CPython 的全局解释器锁（GIL）阻止了同时多线程执行代码，成为了在多核 CPU 上提高 Python 代码运行效率的一大障碍，消除这一障碍是好事，但这也有可能会破坏现有的扩展模块，或显著降低性能以及可维护性。而第三方软件包生态系统是 Python 的一大优势，Python 项目在实现自由线程时需要谨慎，需要避免破坏这一优势。推进 PEP 703 需要将其纳入主线，作为定期发布版本的一部分推出。Python 指导委员计划分成三个阶段：实验阶段，支持但不默认阶段，默认阶段。<p></p>
</div>
