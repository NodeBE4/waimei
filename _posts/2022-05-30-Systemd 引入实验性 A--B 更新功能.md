---
layout: post
title: "Systemd 引入实验性 A/B 更新功能"
date: 2022-05-30T11:30:02.000Z
author: Solidot
from: https://www.solidot.org/story?sid=71679
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1653910202000-->
[Systemd 引入实验性 A/B 更新功能](https://www.solidot.org/story?sid=71679)
------

<div>
如何确保操作系统的<a href="https://linux.slashdot.org/story/22/05/28/194237/newest-version-of-systemd-includes-experimental-feature-for-ab-style-updating" target="_blank">更新平稳且安全</a>？包括 ChromeOS 和  Android 11 在内的系统使用了 A/B 分区机制去实现无缝更新。A 和 B 分区是彼此的拷贝。一个活跃一个闲置，应用更新到闲置的分区。当闲置的分区完成更新，系统会要求重启，然后切换活跃的分区。如果更新出现问题，那么系统可以回滚到旧版本。在新的更新可用时再次尝试。systemd 首席架构师 Lennart Poettering 宣布最新版本引入<a href="https://0pointer.net/blog/fitting-everything-together.html">实验性 A/B 更新功能</a>。
</div>
