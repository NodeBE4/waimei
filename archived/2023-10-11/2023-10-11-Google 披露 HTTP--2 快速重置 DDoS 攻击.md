---
layout: post
title: "Google 披露 HTTP/2 快速重置 DDoS 攻击"
date: 2023-10-11T04:45:51.000Z
author: Solidot
from: https://www.solidot.org/story?sid=76301
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1696999551000-->
[Google 披露 HTTP/2 快速重置 DDoS 攻击](https://www.solidot.org/story?sid=76301)
------

<div>
Google 披露了峰值攻击流量每秒请求数超过 3.98 亿次的 DDoS 攻击，称其全球负载均衡基础设施阻止了这一攻击，客户基本未受影响。这次攻击使用了新颖的 HTTP/2 快速重置方法。Google 称 HTTP/2 的主要设计目标是效率，但这也让 DDoS 的攻击效率更高。HTTP/2 将一个 TCP 连接分为若干个流（Stream），每个流中可以传输若干消息（Message），每个消息由若干最小的二进制帧（Frame）组成。HTTP/1.1 是串行处理每个请求，而 HTTP/2 的客户端在一个 TCP 连接上可以打开多个并发流，在实际使用中客户端每个请求可以打开 100 个流。它允许客户端发送 RST_STREAM 帧告诉服务器取消上一个流。客户端和服务器端无需为此进行协商，客户端可以单方面要求取消上一个流。HTTP/2 快速重置攻击就是利用这一原理。客户端一次连接打开大量流，然后再立即取消每个请求。立即重置流的能力允许每个连接有无数个运行中的请求。请求数量不依赖于 RTT 而是可用网络带宽。<p></p>
</div>
