---
layout: post
title: "Firefox Linux 版本的图形栈将从 GLX 切换到 EGL"
date: 2021-10-31T11:24:23.000Z
author: Solidot
from: https://www.solidot.org/story?sid=69441
tags: [ Solidot ]
categories: [ Solidot ]
---
<!--1635679463000-->
[Firefox Linux 版本的图形栈将从 GLX 切换到 EGL](https://www.solidot.org/story?sid=69441)
------

<div>
即将发布 Firefox 94，其 Linux 版本的图形栈<a href="https://mozillagfx.wordpress.com/2021/10/30/switching-the-linux-graphics-stack-from-glx-to-egl/" target="_blank">将从 GLX 切换到 EGL</a>，但由于驱动问题还不会对所有 Linux 用户默认启用 EGL。为了使用硬件加速 API 如 OpenGL，X11 或 Wayland 等视窗系统都需要一个接口，在 X11 系统上利用 OpenGL 大部分程序都使用 GLX，GLX 诞生于 1990 年代，EGL 是它的继任者，被 Wayland 等广泛使用。但 X11 系统上的普及度比较缓慢，随着 bug 的修复，对 EGL 支持的改进，从 Firefox 94 起，使用 Mesa 驱动版本&gt;21 的用户，EGL 将默认启用。使用私用 Nvidia 驱动的用户则需要<a href="https://bugzilla.mozilla.org/show_bug.cgi?id=1731172">继续等待</a>。
</div>
