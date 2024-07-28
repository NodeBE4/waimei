---
layout: post
title: "Let's Encrypt 计划停止支持 OCSP"
date: 2024-07-26T14:49:09.000Z
author: Solidot
from: https://www.solidot.org/story?sid=78812
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1722005349000-->
[Let's Encrypt 计划停止支持 OCSP](https://www.solidot.org/story?sid=78812)
------

<div>
Let's Encrypt 宣布，出于隐私考虑它计划尽可能快的停止支持 Online Certificate Status Protocol(OCSP)。OCSP 设计作为 Certificate Revocation Lists (CRLs)的轻量级替代，不需要下载完整 CRL 列表就可以检查证书是否有效。但它存在隐私方面的问题，当用户通过 OCSP 检查证书有效性时，运营 OCSP 响应器的 CA 机构会知道用户通过哪个 IP 访问了哪个网站。Let's Encrypt 认为，CA 机构可能会因为法律要求强制收集此类信息，而 CRL 不存在该问题。所有现代浏览器都支持 CRL，因此停止支持 OCSP 不会对终端用户有任何影响。<p></p>
</div>
