---
layout: post
title: "详解 AMD 的 Phoenix SoC"
date: 2023-09-17T15:44:32.000Z
author: Solidot
from: https://www.solidot.org/story?sid=76107
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1694965472000-->
[详解 AMD 的 Phoenix SoC](https://www.solidot.org/story?sid=76107)
------

<div>
AMD 的移动和小型化之路异常艰难。2010 年代初它的 Bulldozer 架构 CPU 对英特尔的产品构不成任何挑战。Zen 架构 CPU 的推出缩小了差距，但还有很多工作要做。其处理器的待机功耗仍然比英特尔差，GPU 在收购 ATI 之后强于英特尔，但集成的 GPU 核心是基于早已过时的架构。AMD 在 2021 年推出的 Ryzen 7 5800H 集成的是基于 GCN 的 Vega GPU，而当时 AMD 已经推出了基于新一代架构 RDNA 2 的 GPU。AMD 新一代产品扭转了这一情况。Steam Deck APU 使用的 Van Gogh 和 Rembrandt 都集成 RDNA 2 GPU，基于 Zen 4 的 Phoenix SoC  则集成了最新一代的 RDNA 3 GPU。除此之外，Phoenix 还集成了多个旨在改进特定应用功耗的加速器，其中 XDNA 加速器能帮助机器学习推理，音频控制器减轻 CPU 的信号处理负担，以及视频引擎支持 AV1 编解码器。XDNA 加速器的 BF16 支持 5 TFLOPS 吞吐量，L2 内存 2MB，通过 DMA 访问系统内存。如果应用能利用 XDNA，它处理 AI 工作负荷的效率要高于 GPU。<p></p>
</div>
