---
layout: post
title: "国产 APP 利用 Android 漏洞提权使其难以卸载 "
date: 2023-03-03T12:07:53.000Z
author: Solidot
from: https://www.solidot.org/story?sid=74293
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1677845273000-->
[国产 APP 利用 Android 漏洞提权使其难以卸载](https://www.solidot.org/story?sid=74293)
------

<div>
国内的一个独立安全研究机构 DarkNavy 发表文章披露，国内一家互联网巨头的 APP 利用了 Android 系统漏洞提权使其难以卸载。报道没有公开相关公司的名字，但称得上巨头也就那四五家公司。报道称，该 APP 首先利用了多个厂商 OEM 代码中的反序列化漏洞提权，提权控制手机系统之后，该 App 即开启了一系列的违规操作，绕过隐私合规监管，大肆收集用户的隐私信息（包括社交媒体账户资料、位置信息、Wi-Fi 信息、基站信息甚至路由器信息等）。之后，该 App 利用手机厂商 OEM 代码中导出的 root-path FileContentProvider， 进行 System App 和敏感系统应用文件读写；进而突破沙箱机制、绕开权限系统改写系统关键配置文件为自身保活，修改用户桌面(Launcher)配置隐藏自身或欺骗用户实现防卸载；随后，还进一步通过覆盖动态代码文件的方式劫持其他应用注入后门执行代码，进行更加隐蔽的长期驻留；甚至还实现了和间谍软件一样的遥控机制，通过远端“云控开关”控制非法行为的启动与暂停，来躲避检测。<p></p>
</div>
