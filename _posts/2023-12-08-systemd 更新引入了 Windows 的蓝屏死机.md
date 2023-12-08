---
layout: post
title: "systemd 更新引入了 Windows 的蓝屏死机"
date: 2023-12-08T06:40:14.000Z
author: Solidot
from: https://www.solidot.org/story?sid=76834
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1702017614000-->
[systemd 更新引入了 Windows 的蓝屏死机](https://www.solidot.org/story?sid=76834)
------

<div>
Windows 臭名昭著的蓝屏死机（BSOD）进入到了 Linux 世界。BSOD 其实是一个展示错误信息的诊断工具，只不过早期 Windows&nbsp; 的 BSOD 代码太模糊而毫无意义。这并不意味着 BSOD 本身是一个糟糕的主意。Linux 的初始化工具 systemd 释出了 v255 版本，引入了一个实验性的组件 systemd-bsod，当 Linux 系统发生引导错误，它会显示一个显示错误代码的全屏信息（即 BSOD），和 Windows 的 BSOD 类似，它也会生成二维码，方便在手机上查找。systemd 的作者 Lennart Poettering 如今在为微软工作。<p></p>
</div>
