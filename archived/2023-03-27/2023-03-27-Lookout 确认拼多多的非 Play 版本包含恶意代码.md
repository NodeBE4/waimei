---
layout: post
title: "Lookout 确认拼多多的非 Play 版本包含恶意代码"
date: 2023-03-27T13:35:30.000Z
author: Solidot
from: https://www.solidot.org/story?sid=74503
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1679924130000-->
[Lookout 确认拼多多的非 Play 版本包含恶意代码](https://www.solidot.org/story?sid=74503)
------

<div>
本月早些时候，独立安全研究机构 DarkNavy 发表文章披露，国内一家互联网巨头的 APP 利用了 Android 系统漏洞提权使其难以卸载。这家巨头之后确认为拼多多。上周一 Google 将拼多多的多个应用标记为恶意程序。拼多多则发表声明，表示强烈反对一位匿名独立安全研究员关于其应用恶意的推测和指控。现在，安全公司 Lookout 的研究人员对非 Google Play 版本的拼多多应用的分析确认了 DarkNavy 的指控。初步分析显示，至少两个非 Play 版本的拼多多应用利用了漏洞  CVE-2023-20963。该漏洞是 Google 在 3 月 6 日公开的，利用该漏洞可以提权，而且整个过程不需要用户交互。两周前修复补丁才提供给终端用户。 Lookout 的研究人员分析了拼多多在 3 月 5 日前发布的两个版本，都包含了利用  CVE-2023-20963 的代码。这两个版本都使用了与拼多多 Google Play 版本相同的密钥签名。目前没有证据表明  Play Store 和苹果 App Store 的版本含有恶意代码，通过 Google 和苹果官方商店下载的拼多多应用是安全的。但通过第三方市场下载的 Android 用户则没有那么幸运了，鉴于拼多多有数亿用户，受影响的用户数量可能是非常惊人。<p></p>
</div>
