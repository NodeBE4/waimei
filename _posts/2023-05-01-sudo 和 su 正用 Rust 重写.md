---
layout: post
title: "sudo 和 su 正用 Rust 重写"
date: 2023-05-01T13:55:06.000Z
author: Solidot
from: https://www.solidot.org/story?sid=74836
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1682949306000-->
[sudo 和 su 正用 Rust 重写](https://www.solidot.org/story?sid=74836)
------

<div>
在亚马逊 AWS 的资助下，类 Unix 操作系统广泛使用的工具 sudo 和 su 正用 Rust 语言重写，以提高软件在内存方面的安全性，进一步增强 Linux 和开源生态系统的安全性。sudo 的开发始于 1980 年代，过去几十年里它已经成为一种必不可少的工具，但它是用 C 语言编写的，遭遇过许多与内存安全问题相关的漏洞。为了确保关键软件的安全性，防止内存安全漏洞，Ferrous Systems 和 Tweede Golf 正在联合将 sudo 从 C 移植到 Rust，他们的项目  sudo-rs 托管在 GitHub 上。<p></p>
</div>
