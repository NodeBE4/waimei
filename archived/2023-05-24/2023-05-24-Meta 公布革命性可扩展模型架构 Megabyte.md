---
layout: post
title: "Meta 公布革命性可扩展模型架构 Megabyte"
date: 2023-05-24T15:46:28.000Z
author: Solidot
from: https://www.solidot.org/story?sid=75047
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1684943188000-->
[Meta 公布革命性可扩展模型架构 Megabyte](https://www.solidot.org/story?sid=75047)
------

<div>
Meta 公司的 AI 研究人员在预印本平台 arXiv 上发表论文《MEGABYTE: Predicting Million-byte Sequences with Multiscale Transformers》，提出了一种革命性的可扩展模型架构 Megabyte。今天的高性能生成式 AI 模型如 OpenAI 的 GPT-4，都是基于 Google 研究人员在 2017 年提出的 Transformer 架构。Meta 的研究人员认为 Transformer 架构可能达到了其阈值，它有两大设计缺陷：第一，随着输入输出长度的增加，自我关注显著扩大。Transformer 语言模型需要注意所有单词，当需要处理的单词量数以千计，计算非常密集。第二，前馈神经网络存在扩展性难题。Megabyte 模型提出了一种不同的架构，它将输入输出序列分割为“补丁（patches）”而不是个别的令牌（tokens）。在每个补丁中，局域 AI 生成结果，全局模型管理协调所有补丁的最终输出，从而解决了扩展性问题。Megabyte 能并行进行计算，相比下传统 Transformers 是串行计算。测试显示，有 15 亿参数的 Megabyte 模型比有 3.5 亿参数的 Transformers 模型生成序列快 40%。Megabyte 模型能支持最多 120 万个令牌，相比下 GPT-4 是 3.2 万个令牌，Anthropic 的 Claude 是 10 万个令牌。<p></p>
</div>
