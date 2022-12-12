---
layout: post
title: "DeepMind 的 AlphaCode 在编程竞赛中达到人类水平"
date: 2022-12-12T06:28:17.000Z
author: Solidot
from: https://www.solidot.org/story?sid=73624
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1670826497000-->
[DeepMind 的 AlphaCode 在编程竞赛中达到人类水平](https://www.solidot.org/story?sid=73624)
------

<div>
根据发表在《科学》期刊上的一项研究，DeepMind 的 AlphaCode 在编程竞赛中达到了人类水平。AlphaCode 首先使用了 GitHub 上的庞大代码库进行训练，熟悉语法和编码规范。然后收集编程竞赛的数千个问题，训练它将问题描述翻译到代码。举个例子，要求编写程序确定长度为 n 的二进制字符串（0 和 1 序列）中没有任何连续 0 的数量。当遇到新问题时，AlphaCode 会用 Python 或 C++ 编写出候选的编程方案，过滤掉不好的。AlphaCode 能生成多达百万个候选编程方案。为了过滤掉如此多的编程方案，它只保留通过测试用例的 1% 程序。为了进一步缩小范围，它会根据程序的输出与虚拟输入的相似性分群，从最大的群开始逐一递交程序，直到找到成功的程序或达到最大递交限额的 10 个程序。这让它能测试广泛的编程策略。经过训练 AlphaCode 解决了 34% 的指定问题。在至少 5000 人参加的在线编程竞赛中，它的表现超过了 45.7% 的程序员。<p></p>
</div>
