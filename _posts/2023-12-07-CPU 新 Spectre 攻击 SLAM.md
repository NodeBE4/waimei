---
layout: post
title: "CPU 新 Spectre 攻击 SLAM"
date: 2023-12-07T14:13:14.000Z
author: Solidot
from: https://www.solidot.org/story?sid=76831
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1701958394000-->
[CPU 新 Spectre 攻击 SLAM](https://www.solidot.org/story?sid=76831)
------

<div>
现代 CPU 的 64 位指针寻址空间远多于需求，因此主要 CPU 供应商都提供了一种机制，将部分地址位用于储存其它数据：英特尔是线性地址掩码(LAM），AMD 是高位地址忽略，Arm 是顶部字节忽略。研究人员报告了被称为 SLAM 的新 Spectre 攻击，利用这些机制绕过指针有效性检查。对于 SLAM 攻击，英特尔计划未来发布相关软件指南，Linux 工程师开发了补丁在软件指南发布前默认禁用 LAM，ARM 发布了类似的声明，AMD 则表示现有的  Spectre v2 补丁能解决 SLAM 攻击。<p></p>
</div>
