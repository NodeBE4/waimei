---
layout: post
title: "Google 用 Rust 重写 Android 的 Binder "
date: 2023-11-02T15:23:04.000Z
author: Solidot
from: https://www.solidot.org/story?sid=76518
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1698938584000-->
[Google 用 Rust 重写 Android 的 Binder](https://www.solidot.org/story?sid=76518)
------

<div>
Google 工程师正在用 Rust 语言重新实现 Android 的 Binder。Binder 是 Android 软件栈的关键部分，负责进程间通信(IPC) 等任务，对沙盒策略至关重要 ，此前是用 C 语言写的，为了提高鲁棒性（robustness）和安全性，Google 使用内存安全语言 Rust 进行重写。工程师称，用 Rust 有助于在降低复杂度的同时不会增加安全风险，它还可以防止诸如引用计数、锁定、边界检查等错误。binderfs 文件系统组件仍然保留 C 语言版本，重写它的工作量太大，价值也不高。<p></p>
</div>
