---
layout: post
title: "Google 宣布安全操作系统 KataOS 及其实现 Sparrow"
date: 2022-10-17T10:08:23.000Z
author: Solidot
from: https://www.solidot.org/story?sid=73080
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1666001303000-->
[Google 宣布安全操作系统 KataOS 及其实现 Sparrow](https://www.solidot.org/story?sid=73080)
------

<div>
Google <a href="https://opensource.googleblog.com/2022/10/announcing-kataos-and-sparrow.html">宣布</a>了新操作系统 KataOS 及其参考实现 Sparrow，搜索巨人旨在创造一种安全的嵌入式系统。<a href="https://github.com/AmbiML/sparrow-manifest">项目源代码</a>托管在 GitHub 上，采用 Apache License 2.0 许可证。Google 称我们身边的智能设备愈来愈多，因此需要一种简单的方案为嵌入式硬件构建可验证的安全系统。它的新操作系统 KataOS 使用了 seL4 微内核，它已经在数学上被证明是安全的。系统几乎完全用 Rust 语言实现，核心部分包括包括提供系统调用 API 的 sel4-sys crate，替代 rootserver 等。Google 还与 Antmicro 合作开发了模拟器 <a href="https://antmicro.com/blog/2022/08/running-rust-programs-in-sel4/" target="_blank">Renode</a>。
</div>
