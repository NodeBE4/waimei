---
layout: post
title: "Firefox 如何改进在 Windows 平台的稳定性"
date: 2022-11-24T06:05:35.000Z
author: Solidot
from: https://www.solidot.org/story?sid=73465
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1669269935000-->
[Firefox 如何改进在 Windows 平台的稳定性](https://www.solidot.org/story?sid=73465)
------

<div>
内存问题是 Windows 版 Firefox 发生崩溃的主要原因。Windows 上运行的应用程序比其它操作系统上的程序更容易发生内存耗尽问题，这与 Windows 处理内存的方式有关。现代操作系统都允许应用分配一块地址空间，当应用使用其保留的地址空间时，系统会用一块物理内存支持它，如果需要会交换部分现有数据。Linux 和 macOS  都是如此工作，但 Windows 多了一个步骤。它需要应用在请求使用其保留的地址空间前先递交使用范围，确保系统能找到可用物理内存。Windows 为此限制了递交内存用量在物理内存和交换文件大小之和内。这种递交空间（commit space）是应用面对的硬限制。达到这个限制，内存分配会失败。Firefox 开发者在分析浏览器崩溃问题时发现用户机器上的可用物理内存仍然很多，但递交空间却耗尽了。他们不知道为什么会发生这种情况，但认为可以用一些技巧规避这一问题：当内存分配失败时，浏览器不是立即崩溃，而是先等待下，然后尝试重新内存分配。这会导致浏览器卡住短暂的几分之一秒，但比崩溃好得多。Firefox&nbsp; 105 中应用了这一技巧，显著改进了浏览器的稳定性。<p></p>
</div>
