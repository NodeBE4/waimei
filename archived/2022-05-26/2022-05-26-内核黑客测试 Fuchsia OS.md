---
layout: post
title: "内核黑客测试 Fuchsia OS"
date: 2022-05-26T10:55:00.000Z
author: Solidot
from: https://www.solidot.org/story?sid=71646
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1653562500000-->
[内核黑客测试 Fuchsia OS](https://www.solidot.org/story?sid=71646)
------

<div>
专注于 Linux 内核安全的黑客 Alexander Popo <a href="https://a13xp0p0v.github.io/2022/05/24/pwn-fuchsia.html" target="_blank">研究了 Google 开发的全新操作系统 Fuchsia OS</a>，从攻击者的角度评估其安全性。Google 大约是从 2016 年起开始开发 Fuchsia，2020 年 12 月允许外部开发者参与该项目，2021 年 5 月向 Nest Hub 设备推送 Fuchsia。Fuchsia 是为联网设备如物联网、智能手机等设计的，特别强调了安全性和可升级性。它没有用户的概念，而是基于能力（apability-based），类似给网页分配一个网址 URL，使用 URL(授权的能力)你可以访问网页的内容，但你无法获得另一个 URL（另一个未授权给你的能力）。运行在 Fuchsia 上的软件通常只能获得完成工作所需的最小能力，因此 Fuchsia 的本地提权概念不同于 Linux 操作系统。Fuchsia 是基于名叫 Zircon 微内核，许多功能都转移到了用户空间，因此攻击面更小。但 Zircon 并没有达到最简化，有逾 170 个系统调用，远多于典型的微内核。Fuchsia 另一个安全特性是沙盒化，应用程序和系统服务都以名为组件（components）的独立软件单元形式存在，这些组件运行在隔离的沙盒内，它也没有全局的文件系统。
</div>
