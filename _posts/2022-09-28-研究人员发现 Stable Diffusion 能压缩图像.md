---
layout: post
title: "研究人员发现 Stable Diffusion 能压缩图像"
date: 2022-09-28T06:42:02.000Z
author: Solidot
from: https://www.solidot.org/story?sid=72903
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1664347322000-->
[研究人员发现 Stable Diffusion 能压缩图像](https://www.solidot.org/story?sid=72903)
------

<div>
瑞士软件工程师 Matthias Bühlmann 发现，流行的 AI 自然语言图像合成模型 Stable Diffusion <a href="https://arstechnica.com/information-technology/2022/09/better-than-jpeg-researcher-discovers-that-stable-diffusion-can-compress-images/">能用于压缩位图图像</a>，在高压缩率下比 JPEG 或 WebP 有更少的视觉瑕疵，缺陷是可能会添加原图不存在的东西。Stable Diffusion 利用互联网上数百万张图片进行训练，能根据文本描述或提示生成图像。在训练过程中，它在图像和相关词语之间进行统计关联，对每张图像提取出较少的关键信息表述，将其作为“权重（weights）”储存。绝大部分用户在使用 Stable Diffusion 时是通过文本描述去生成图像，但 Bühlmann 剔除了文本编码器，强行让图像通过 Stable Diffusion 的图像编码器进行处理，能将低精度的图像转变成高精度的潜在空间(latent space)表示，在此过程中大幅减少图像体积。测试显示一张 768KB 的图像用 JPEG 压缩到 5.68KB，用 WebP 压缩到 5.71 KB，而用 Stable Diffusion 压缩到 4.98KB。
</div>
