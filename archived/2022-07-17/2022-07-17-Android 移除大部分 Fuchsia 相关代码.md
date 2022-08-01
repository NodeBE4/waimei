---
layout: post
title: "Android 移除大部分 Fuchsia 相关代码"
date: 2022-07-17T10:44:47.000Z
author: Solidot
from: https://www.solidot.org/story?sid=72148
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1658054687000-->
[Android 移除大部分 Fuchsia 相关代码](https://www.solidot.org/story?sid=72148)
------

<div>
过去几年，Google 投入数以十亿美元计的资金开发名为 Fuchsia 的全新操作系统，但至今为止其成果寥寥无几。Fuchsia 唯一的成果是作为 Nest 设备的底层操作系统使用，Google 曾尝试让 Fuchsia 能运行 Android 应用，为此它在 Android Open Source Project(AOSP) 创建了一个项目 device/google/fuchsia，设计为 Fuchsia 设备构建 Android  运行时。但本周该项目下的所有代码<a href="https://9to5google.com/2022/07/15/android-removes-fuchsia-code-starnix/">都被删除</a>，取而代之的是一条 TODO 信息，Google 可能会用其它项目取代它。负责该变更的开发者来自 Fuchsia 的 Starnix 项目。Starnix 于 2021 年创建，旨在让 Fuchsia 能原生运行为 Linux 或 Android 构建的应用或库。
</div>
