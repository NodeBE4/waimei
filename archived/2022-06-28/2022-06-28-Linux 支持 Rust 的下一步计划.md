---
layout: post
title: "Linux 支持 Rust 的下一步计划"
date: 2022-06-28T14:48:19.000Z
author: Solidot
from: https://www.solidot.org/story?sid=71965
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1656427699000-->
[Linux 支持 Rust 的下一步计划](https://www.solidot.org/story?sid=71965)
------

<div>
在 Linux 基金会举办的开源峰会上，Linus Torvalds 谈到了 Rust 语言合并到内核的可能性，<a href="https://www.solidot.org/story?sid=71927">表示</a>最快可能在 Linux 5.20 开发周期中合并到内核。Linux 内核是用 C 语言开发的，社区没有计划用 Rust 重写内核，而是侧重于用 Rust 开发内核模块如驱动程序。Rust 是一种高性能、内存安全的语言，而软件项目发现的大部分漏洞都属于内存安全相关漏洞，用 Rust 开发驱动将有助于改进内核的内存安全。Rust 开发者 Miguel Ojeda 发表博文介绍了 <a href="https://www.memorysafety.org/blog/memory-safety-in-linux-kernel/" target="_blank">Linux 支持 Rust 的下一步计划</a>：示例驱动，稳定 Rust 功能，用 GCC 编译内核 Rust 代码，等等。
</div>
