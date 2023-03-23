---
layout: post
title: "Rust for Linux 维护者谈未来计划"
date: 2023-03-08T06:48:02.000Z
author: Solidot
from: https://www.solidot.org/story?sid=74329
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1678258082000-->
[Rust for Linux 维护者谈未来计划](https://www.solidot.org/story?sid=74329)
------

<div>
Linux 内核从 6.1 开始加入了对 Rust 语言的初步支持，Rust for Linux 维护者 Miguel Ojeda 接受采访，谈论项目的现状和未来。他表示目前的工作主要是为上游加入足够的抽象，为首批 Rust 驱动做好准备。而首批进入上游的驱动可能包括 Asahi Linux 的 GPU 驱动、Android 的 Binder 和 NVMe 驱动。它们将为未来的 Rust 内核抽象和驱动树立标杆。在此过程中还需要相关的内核维护者参与进来评估和评论代码。一旦 Rust for Linux 准备就绪，内核使用 Rust 的一个明显优点是减少内存相关漏洞。此前的报告显示，七成的漏洞是由于C/C++ 代码库中的内存安全问题导致的。如果使用 Rust 能消除其中大部分或者减轻漏洞的严重程度，那么对终端用户而言意味着安全性改进，需要紧急给内核打补丁的次数减少，企业也可能更少遭到入侵。<br>Asahi Linux 项目已经发布了支持苹果 AGX GPU 处理器的驱动早期版本。<p></p>
</div>
