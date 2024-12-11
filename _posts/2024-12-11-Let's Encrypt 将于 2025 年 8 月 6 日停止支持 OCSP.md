---
layout: post
title: "Let's Encrypt 将于 2025 年 8 月 6 日停止支持 OCSP"
date: 2024-12-11T07:45:24.000Z
author: Solidot
from: https://www.solidot.org/story?sid=80017
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1733903124000-->
[Let's Encrypt 将于 2025 年 8 月 6 日停止支持 OCSP](https://www.solidot.org/story?sid=80017)
------

<div>
Let's Encrypt 宣布将于 2025 年 8 月 6 日停止支持 Online Certificate Status Protocol(OCSP)：从 2025 年 1 月 30 日起，包含 OCSP Must Staple 扩展的签发请求将失败，除非此前签发的证书包含 OCSP Must Staple 扩展；从5 月 7 日起，所有包含 OCSP Must Staple 扩展的签发请求都将失败。Let's Encrypt 是出于隐私考虑决定停止支持 OCSP。OCSP 设计作为 Certificate Revocation Lists (CRLs)的轻量级替代，不需要下载完整 CRL 列表就可以检查证书是否有效。但它存在隐私方面的问题，当用户通过 OCSP 检查证书有效性时，运营 OCSP 响应器的 CA 机构会知道用户通过哪个 IP 访问了哪个网站。Let's Encrypt 认为，CA 机构可能会因为法律要求强制收集此类信息，而 CRL 不存在该问题。所有现代浏览器都支持 CRL，因此停止支持 OCSP 不会对终端用户有任何影响。<p></p>
</div>
