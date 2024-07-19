---
layout: post
title: "Linux DRM Panic 死机屏幕将能支持二维码"
date: 2024-07-04T14:43:10.000Z
author: Solidot
from: https://www.solidot.org/story?sid=78609
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1720104190000-->
[Linux DRM Panic 死机屏幕将能支持二维码](https://www.solidot.org/story?sid=78609)
------

<div>
Linux 6.10 引入了 DRM Panic，提供了类似 Windows 蓝屏死机的功能，在屏幕上显示内核错误信息。但内核错误信息通常很长，尤其是它如果包含堆栈跟踪的话。现在 Red Hat 开发者 Jocelyn Falempe 发布了补丁，提供了将错误信息转换为二维码的功能（类似微软的做法），允许用户通过智能手机扫描去捕捉错误信息，方便以后进行分析，或将其添加到 bug 报告里。Falempe 使用 Rust 语言开发了 DRM Panic QR 代码。他表示没有特殊理由，只是想学习下 Rust。<p></p>
</div>
