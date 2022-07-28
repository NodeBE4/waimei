---
layout: post
title: "Google 如何滚动更新其内部 Linux 发行版"
date: 2022-07-13T15:36:00.000Z
author: Solidot
from: https://www.solidot.org/story?sid=72118
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1657726560000-->
[Google 如何滚动更新其内部 Linux 发行版](https://www.solidot.org/story?sid=72118)
------

<div>
Google 内部使用了多种操作系统，其中包括 Linux。Google 早期使用的内部 Linux 发行版是基于 Ubuntu LTS 的 Goobuntu。Ubuntu LTS 需要每隔两年更新一次，对企业而言日益不便，要在操作系统终止支持前升级逾十万台计算机并非易事，重新安装和重新定制企业计算机既困难也费时间。因此 Google <a href="https://cloud.google.com/blog/topics/developers-practitioners/how-google-got-to-rolling-linux-releases-for-desktops">转向了滚动更新发行版</a>，它没有使用著名的滚动更新发行版如 Arch Linux，而是基于 Debian 将新发行版称为 gLinux Rodete (Rolling Debian Testing)。选择 Debian 是因为它有着庞大的软件包库，庞大的社区，而 Ubuntu 也是基于  Debian，迁移过去更容易。Debian 稳定分支也是差不多两年更新一次，但其测试分支是滚动更新的。滚动更新需要尽可能防止新版本对现有工作流程造成破坏，Google 引入了名为 Sieve 的工作流系统，使用虚拟化测试套装确保软件包新版本不会破坏核心组件和开发者的工作流程。Google 表示，Goobuntu 的最后一个版本是基于  Ubuntu 14.04 LTS (Codename Trusty)， Rodete 的开发始于 2015 年，2017 年开始从 Goobuntu 迁移到 Rodete，2018 年底迁移完成，2019 年关闭了剩余的 Goobuntu 机器。
</div>
