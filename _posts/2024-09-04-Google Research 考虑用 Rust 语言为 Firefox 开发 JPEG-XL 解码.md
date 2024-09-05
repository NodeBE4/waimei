---
layout: post
title: "Google Research 考虑用 Rust 语言为 Firefox 开发 JPEG-XL 解码器"
date: 2024-09-04T16:32:02.000Z
author: Solidot
from: https://www.solidot.org/story?sid=79166
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1725467522000-->
[Google Research 考虑用 Rust 语言为 Firefox 开发 JPEG-XL 解码器](https://www.solidot.org/story?sid=79166)
------

<div>
2023 年 Google Chrome 移除了对实验性的 JPEG-XL 图像格式的支持。JPEG-XL 是免专利的新兴图像格式。Google 此举引发了很多争议，因为 Chrome/Chromium 占据了九成市场份额，它是 Web 标准事实上的仲裁者。一年之后，事情有望发生戏剧性转变。Google Research 的 JPEG-XL 团队与 Mozilla 过去几个月展开了富有成效的对话，围绕的主题是用 Rust 语言为 Firefox 开发 JPEG-XL 解码器。Rust 是内存安全语言，而 JPEG-XL 的参考解码器包含了逾十万行多线程 C++ 代码，它可能会增加浏览器的攻击面。如果 Rust 版本的解码器在 Firefox 上的实验取得成功，也许 Google Chrome 会重新考虑对 JPEG-XL 的支持。如果 Rust 版本的解码器只供 Firefox 使用，将会是非常有讽刺意味的。<p></p>
</div>
