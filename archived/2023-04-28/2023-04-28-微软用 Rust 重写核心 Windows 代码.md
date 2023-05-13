---
layout: post
title: "微软用 Rust 重写核心 Windows 代码"
date: 2023-04-28T07:29:14.000Z
author: Solidot
from: https://www.solidot.org/story?sid=74821
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1682666954000-->
[微软用 Rust 重写核心 Windows 代码](https://www.solidot.org/story?sid=74821)
------

<div>
微软正在用 Rust 语言重写核心 Windows 库，开始将其提供给开发者使用。Windows 操作系统安全总监 David "dwizzle" Weston 上个月在以色列特拉维夫举行的 BlueHat IL 2023 上宣布了 Rust 代码进入内核的消息。微软的基本目标是将内部 C++ 数据类型替换成 Rust。Rust 是一种高性能、内存安全语言，而软件项目的大部分漏洞都属于内存安全 bug。自 2006 年以来微软在 Windows 中修复的漏洞大约七成是内存安全漏洞。Windows 的 Rust 重写始于 2020 年的 DWriteCore，它是用于文本分析、布局和渲染的 DWrite 引擎的 Windows App SDK 实现。DWriteCore 现在包含大约 15.2 万行的 Rust 代码和大约 9.6 万行的 C++ 代码。Windows 的 GUI Win32 GDI 正移植到 Rust，目前包含了 3.6 万行 Rust 代码。Weston 称，Windows 内核的一个系统调用（SysCall）正用 Rust 实现。他表示在可预见的未来用 Rust 语言重写 Windows 还不可能会发生。<p></p>
</div>
