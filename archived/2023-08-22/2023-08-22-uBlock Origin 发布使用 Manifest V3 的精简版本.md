---
layout: post
title: "uBlock Origin 发布使用 Manifest V3 的精简版本"
date: 2023-08-22T04:07:05.000Z
author: Solidot
from: https://www.solidot.org/story?sid=75856
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1692677225000-->
[uBlock Origin 发布使用 Manifest V3 的精简版本](https://www.solidot.org/story?sid=75856)
------

<div>
uBlock Origin 作者 Raymond Hill 发布了 uBlock Origin Lite（uBO Lite），使用新扩展系统 Manifest V3 的精简版本。Google Chrome 正逐步强制推广 Manifest V3 扩展，该扩展系统受争议之处是它将限制 WebRequest API 的功能，用 declarativeNetRequest 替代。广告屏蔽扩展如 uBlock Origin 将会受到影响，因为它们使用 WebRequest 在广告下载前屏蔽其请求。Mozilla 的 Manifest V3 实现既支持 declarativeNetRequest API 又继续支持 webRequest API，uBO Lite 使用了 declarativeNetRequest API 在无需读写权限的情况下提供广告屏蔽功能。uBO 的完整版本仍然使用 webRequest API。uBO Lite 的屏蔽功能弱于完整版。<br><p></p>
</div>
