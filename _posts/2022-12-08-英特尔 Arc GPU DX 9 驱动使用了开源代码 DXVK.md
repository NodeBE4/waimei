---
layout: post
title: "英特尔 Arc GPU DX 9 驱动使用了开源代码 DXVK"
date: 2022-12-08T06:56:12.000Z
author: Solidot
from: https://www.solidot.org/story?sid=73594
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1670482572000-->
[英特尔 Arc GPU DX 9 驱动使用了开源代码 DXVK](https://www.solidot.org/story?sid=73594)
------

<div>
英特尔 Arc GPU 独显在 DX 9 游戏下的性能相当差，它最近对 Arc 的 DX 9 驱动进行了大更新，结果发现新 DX 9 驱动使用了开源代码 DXVK，而英特尔的官方博客根本没有提到 DXVK，只有查看 readme 文件才发现是 DXVK。DXVK 是 Steam Play Proton 的一部分，而 Proton 是 Windows 兼容层项目 Wine 的分支，它能将 Direct3D 9、Direct3D 10 和 Direct3D 11 翻译到 Vulkan，它有 Linux 的原生实现，也支持 Windows。英特尔使用 DXVK 并不太意外，英伟达也在 RTX Remix 中使用了 DXVK。<p></p>
</div>
