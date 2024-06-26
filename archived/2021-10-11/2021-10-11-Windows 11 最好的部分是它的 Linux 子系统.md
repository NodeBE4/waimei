---
layout: post
title: "Windows 11 最好的部分是它的 Linux 子系统"
date: 2021-10-11T11:17:40.000Z
author: Solidot
from: https://www.solidot.org/story?sid=69193
tags: [ Solidot ]
categories: [ Solidot ]
---
<!--1633951060000-->
[Windows 11 最好的部分是它的 Linux 子系统](https://www.solidot.org/story?sid=69193)
------

<div>
微软在 Windows 10 一周年更新中引入了名叫 Windows Subsystem for Linux(WSL) 的 Linux 兼容层，2020 年的 Windows 10 build 2004 升级到了 WSL2。尽管如此，在 Windows 上使用 Linux 面临两大障碍：安装 WSL 没有本应该做到的那么容易，安装 Linux 图形应用也不轻松。<a href="https://arstechnica.com/gadgets/2021/10/the-best-part-of-windows-11-is-a-revamped-windows-subsystem-for-linux/" target="_blank">Windows 11 解决了这两大问题</a>，WSL 仍然不完美，但比之前有了巨大的进步。从 Windows 10 build 2004 开始，用户只需要在命令提示符下输入 wsl --install 就可以安装 WSL，Windows 11 没有改变这一方法，输入 wsl --install 就能安装 Hyper-V、WSL 和当前版本的 Ubuntu。如果想使用其它发行版如 openSUSE 只需要输入 wsl --install -d openSUSE-42，或者通过 wsl --list --online 寻找可用发行版然后输入 wsl --install -d distroname 安装你选择的发行版。安装第二个发行版不会覆盖第一个发行版，不同发行版之间的运行环境是隔离的。除了易于安装外，Windows 11 的 WSL 还加入了对图形应用和音频的支持，是首个支持 WSLg 的 Windows 系统。
</div>
