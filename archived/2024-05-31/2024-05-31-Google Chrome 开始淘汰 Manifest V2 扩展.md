---
layout: post
title: "Google Chrome 开始淘汰 Manifest V2 扩展"
date: 2024-05-31T09:24:57.000Z
author: Solidot
from: https://www.solidot.org/story?sid=78321
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1717147497000-->
[Google Chrome 开始淘汰 Manifest V2 扩展](https://www.solidot.org/story?sid=78321)
------

<div>
Google Chrome 官方博客宣布开始淘汰 Manifest V2 扩展：从 2024 年 6 月 3 日起在 Chrome Dev、Canary 和 Beta 渠道，如果用户仍然安装有 Manifest V2 扩展，那么用户访问扩展管理页面 chrome://extensions 时会显示警告信息，通知他们 Manifest V2 扩展将很快不予支持。未来几个月 Manifest V2 扩展将逐步禁用，用户将会被导向扩展商店 Chrome Web Store 推荐 Manifest V3 替代扩展。短时间内禁用的 Manifest V2 扩展可以重新启用，但未来将会被彻底禁用。对于受争议的 Manifest V3 扩展系统，Google 声称 Chrome Web Store 中逾 85% 的活跃支持扩展已经迁移到 Manifest V3。 Manifest V3 受争议之处是它限制了 WebRequest API 的功能，用 declarativeNetRequest 替代了 WebRequest。广告屏蔽扩展如 uBlock Origin 会受到影响，因为它们使用 WebRequest 在广告下载前屏蔽其请求。禁用 Manifest V2 扩展意味着 uBlock Origin 会被禁用。开发者已经释出了使用 Manifest V3 的精简版本 uBO Lite，其功能弱于原版。原版未来只能在 Firefox 等浏览器上使用。<p></p>
</div>
