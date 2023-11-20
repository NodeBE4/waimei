---
layout: post
title: "Firefox 用户访问 YouTube 时人为加入了 5 秒加载延迟"
date: 2023-11-20T12:14:08.000Z
author: Solidot
from: https://www.solidot.org/story?sid=76670
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1700482448000-->
[Firefox 用户访问 YouTube 时人为加入了 5 秒加载延迟](https://www.solidot.org/story?sid=76670)
------

<div>
一位 Mozilla Firefox 用户在 Reddit 论坛上报告了一个异常情况：在新标签页打开一个 YouTube 视频时不知为何加载超级慢。其他 Firefox 用户很快发现 YouTube 的 polymer 脚本中有一行人为引入 5 秒加载延迟的代码：“setTimeout(function(){c();a.resolve(1)},5E3);”，根据上下文，该代码被认为是 YouTube 最近采取的反广告屏蔽扩展的功能的一部分。使用流行广告屏蔽扩展 UBO 的用户可以在过滤器中加入“www.youtube.com##+js(nano-stb, resolve(1), *, 0.001)”来绕过这段恼人的加载延迟。<p></p>
</div>
