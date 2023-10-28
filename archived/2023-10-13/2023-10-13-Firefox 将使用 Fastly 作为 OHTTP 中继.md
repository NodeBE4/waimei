---
layout: post
title: "Firefox 将使用 Fastly 作为 OHTTP 中继"
date: 2023-10-13T13:02:10.000Z
author: Solidot
from: https://www.solidot.org/story?sid=76334
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1697202130000-->
[Firefox 将使用 Fastly 作为 OHTTP 中继](https://www.solidot.org/story?sid=76334)
------

<div>
云计算服务商 Fastly 宣布与 Mozilla 合作，Firefox 将使用 Fastly 作为 OHTTP 中继。OHTTP 代表 Oblivious HTTP，旨在加强网络连接的隐私性。传统的 HTTP 请求包含了能用于识别用户身份的元数据，比如浏览器的 User-Agent、网络信息如 AS(自治系统)和 IP 地址，这些信息组合起来能用于去匿名化用户身份。OHTTP 架构包含四层：客户端封装和加密旨在发送给目标的请求，但不是直接发送给目标，而是先发送给中继；中继在移除客户端的身份信息之后发送给网关，请求是加密的，它并不拥有密钥，因此不知道请求内容；网关收到去除隐私信息的请求版本之后对其进行解密和解封装，然后发送给目标；目标就是标准的 HTTP 服务，但不会收到客户端可能的身份信息。OHTTP 通过这种方法处理 HTTP 请求去加强隐私。当然不喜欢该功能的用户可以在 Firefox 工具栏输入 about:config 禁用 network.trr.use_ohttp（目前默认禁用）。<p></p>
</div>
