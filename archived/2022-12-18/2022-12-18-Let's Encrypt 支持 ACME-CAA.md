---
layout: post
title: "Let's Encrypt 支持 ACME-CAA"
date: 2022-12-18T14:58:26.000Z
author: Solidot
from: https://www.solidot.org/story?sid=73685
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1671375506000-->
[Let's Encrypt 支持 ACME-CAA](https://www.solidot.org/story?sid=73685)
------

<div>
Let's Encrypt 宣布支持 ACME-CAA(Certification Authority Authorization)——它是 DNS CAA 记录的一个扩展，旨在堵上 Domain Validation（域名验证）的漏洞。SSL 证书的一个主要目的是限制中间人攻击。而当你从 CA 如 Let's Encrypt 为一个域名申请证书，Let's Encrypt 必须采取措施确认你是域名的合法所有者。域名验证的方法通常是 CA 生成随机的质询字符串，要求你将其托管在自己的域名上。如果你成功的完成了这一要求，那么意味着你控制着该域名，因此是域名的合法运营者。问题是在执行域名验证时你还没有 SSL 证书，也就是说 CA 验证你的域名是通过 HTTP 而不是 HTTPS，这意味着整个域名验证过程容易遭到中间人攻击。ACME-CAA 就是设计堵上漏洞，要求 CAA 记录指向 Let’s Encrypt 的一个特定帐户名。<p></p>
</div>
