---
layout: post
title: "DeepMind 的 AlphaTensor 找到更快的矩阵乘法算法"
date: 2022-10-09T08:50:39.000Z
author: Solidot
from: https://www.solidot.org/story?sid=72993
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1665305439000-->
[DeepMind 的 AlphaTensor 找到更快的矩阵乘法算法](https://www.solidot.org/story?sid=72993)
------

<div>
Google 子公司 DeepMind 的研究人员在《自然》期刊上发表<a href="https://www.nature.com/articles/d41586-022-03166-w">论文</a>，<a href="https://news.sciencenet.cn/htmlnews/2022/10/487400.shtm">报告</a>了名为 <a href="https://www.deepmind.com/blog/discovering-novel-algorithms-with-alphatensor" target="_blank">AlphaTensor</a> 的 AI 找到更快的矩阵乘法算法。数学在计算机编程中经常出现，通常作为描述和操纵现实世界现象表示的一种手段。例如，它用于表示计算机屏幕上的像素、天气状况或人工网络中的节点。在这种情况下，使用数学的主要方式之一，就是对矩阵进行计算。在对游戏进行编程时，矩阵描述了可能的运动选项。为了实现这样的运动，矩阵经常被相乘和/或相加。这需要海量的工作，随着矩阵变得越来越大尤其如此，这就是为什么计算机科学家花费大量时间和精力来开发越来越有效算法来完成工作的原因。1969 年，数学家沃尔克·斯特拉森想出了一种方法，只使用 7 个乘法运算而不是标准的8个乘法运算将两个 2×2 矩阵相乘。DeepMind 研究人员从游戏系统中寻找灵感，这些游戏大多数都是基于强化学习的。在构建了一些初步系统之后，研究小组将重点转向了树搜索，这也用于游戏编程，是系统在特定情况下查看各种方案的一种手段。当应用于乘法矩阵时，研究人员发现，将 AI 系统转换为游戏可搜索最有效的方法来获得所需的结果——数学结果。研究人员通过允许它搜索、评估来测试他们的系统，然后使用现有算法，并以奖励来激励选出最有效的算法。系统学会了影响矩阵乘法效率的因素。接下来，研究人员将允许系统创建自己的算法，寻求进一步提高效率。他们发现，在许多情况下，系统选择的算法比人类前辈创建的算法更好。
</div>
