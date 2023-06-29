---
layout: post
title: "GitHub DDoS 开源网站遭批评"
date: 2023-06-29T08:11:59.000Z
author: Solidot
from: https://www.solidot.org/story?sid=75375
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1688026319000-->
[GitHub DDoS 开源网站遭批评](https://www.solidot.org/story?sid=75375)
------

<div>
GCC 等程序使用的核心算术库 GMP 项目本月中旬披露，它的服务器遭到了来自数百个微软 IP 的攻击。项目主要开发者 Torbjorn Granlund 称，攻击针对的是 GMP 库，使用了数千个相同的请求，这些请求是精心挑选的，目的是让服务器过载。作为紧急响应，GMP 服务器防火墙屏蔽了所有微软 IP 访问。微软 GitHub 威胁捕获、运营和响应总监 Mike Blacker 很快识别了罪魁祸首：一个 GitHub Actions Workflow。一位 GitHub 用户更新了 FFmpeg-Builds 项目的一个脚本，从 https://gmplib.org 上提取内容，该构建被配置在 100 种不同类型的计算机/架构上运行并行同时测试。他认为这位用户的活动看起来并没有恶意目的。Granlund 表示在屏蔽了 100 个微软 IP 段后一周，仍然有来自相同 IP 地址的密集流量，但在防火墙屏蔽之后服务器不再受到影响。他对 Github/微软认为自己不需要承担任何责任表达了不满。<p></p>
</div>
