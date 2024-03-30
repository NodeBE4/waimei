---
layout: post
title: "超微服务器主板 x11ssh-f 的 OpenBMC 移植 (WIP)"
date: 2024-03-15T14:10:46.000Z
author: Solidot
from: https://www.solidot.org/story?sid=77610
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1710511846000-->
[超微服务器主板 x11ssh-f 的 OpenBMC 移植 (WIP)](https://www.solidot.org/story?sid=77610)
------

<div>
Shawn the R0ck 写道：<i>BMC 全称基板管理控制器（baseboard management controller），是一个嵌入某些计算机（通常是服务器）主板的特制微控制器，拥有自己的固件、内存和网络连接（通过自己的独立网卡或网络控制器旁路接口 NC-SI 共享宿主的网卡）。它是承载智能平台管理接口（Intelligent Platform Management Interface，IPMI）的硬件，通过一个扩展自 I²C 的基板管理控制总线/桥（Intelligent Platform Management Bus/Bridge，IPMB）与分布于各个不同系统模块中的卫星控制器相连，可以独立于操作系统监视这些系统模块的工作状态并进行管理，如开关机、感知组件温度并调整风扇转速，甚至可以作为远程控制台，获取屏幕显示并作为键盘鼠标与操作系统交互，甚至模拟外存储器以远程安装操作系统。<br>BMC 之所以能做到如此深度的管理，是因为 BMC 深度连接到宿主系统的总线之中。BMC 经常是取代了一般 x86 计算机系统的 SuperIO 芯片，通过 LPC、SMBUS 总线连接到宿主，并对宿主提供相应功能（如串口、风扇管理等）。为了实现远程控制台和外存储器模拟，BMC 还与宿主的 PCI（E） 总线相连并表现为显卡，作为从设备与宿主的 USB 总线相连以表现为输入设备和外存储器。<br>虽然大部分 BMC 的原厂固件使用了 Linux 内核，但一般用的是十分老旧的版本，且其用户态程序一般不是自由软件，因此私有的 BMC 固件正在被逐步视为安全隐患。为此，和 Linux 基金会合作的 OpenBMC 项目面世了，它是一个面向 BMC 的 GNU/Linux 发行版，提供了可以从源代码编译而出的自由 BMC 软件栈，它使用 Yocto 计划作为编译和发行版生成系统，可以生成能直接刷入 BMC 的 rom 芯片的固件镜像。在其内部，OpenBMC 使用 D-Bus 进行进程间通信，并提供一个 web 应用程序使用户能够与 BMC 软件栈交互。HardenedVault团队尝试把OpenBMC移植到超微x11ssh-f主板上，这是一款支持开放固件coreboot的服务器主板。</i><p></p>
</div>
