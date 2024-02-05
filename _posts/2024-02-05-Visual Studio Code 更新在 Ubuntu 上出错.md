---
layout: post
title: "Visual Studio Code 更新在 Ubuntu 上出错"
date: 2024-02-05T05:39:00.000Z
author: Solidot
from: https://www.solidot.org/story?sid=77308
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1707111540000-->
[Visual Studio Code 更新在 Ubuntu 上出错](https://www.solidot.org/story?sid=77308)
------

<div>
微软最近释出了 Visual Studio Code 最新更新（v1.86 或 2024 年 1 月更新），Ubuntu 用户在 GitHub 问题页面报告编辑器无法启动或停止工作。原因被发现微软将 Visual Studio Code 远程开发工具的最低构建版本升级到了 glibc 2.28，而 Ubuntu 18.04 LTS 使用的版本是 glibc 2.27，这导致编辑器停止工作。Canonical 为 Ubuntu 18.04 LTS 提供了 10 年支持，一直支持到 2028 年，升级一个长期支持版本的重要软件包是不太可能的。因此对 Ubuntu 18.04 LTS 用户而言，唯一的解决方案是降级，安装旧版本。开发者抱怨微软在升级 Visual Studio Code 时本来可以检查下 glibc 的版本号，如果不符合要求就拒绝更新，结果因为它的原因却导致开发者的工作陷入困境。微软已经关闭了 GitHub 问题页的相关讨论，理由是“过激（too heated）”。<p></p>
</div>
