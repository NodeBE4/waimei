---
layout: post
title: "Firefox 将禁用 HTTP/2 服务器推送"
date: 2024-09-06T15:45:00.000Z
author: Solidot
from: https://www.solidot.org/story?sid=79185
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1725637500000-->
[Firefox 将禁用 HTTP/2 服务器推送](https://www.solidot.org/story?sid=79185)
------

<div>
继 Safari 和 Chrome 之后，Firefox 也将禁用 HTTP/2 服务器推送。Chrome 是在两年前禁用 HTTP/2 服务器推送，理由是使用率低，它推荐将 rel="preload" 和 103 Early 作为替代。Firefox 一直支持 HTTP/2 推送，但过去几个月遭遇了与 HTTP/2 推送相关的 bug，原因是使用推送的 webserver 和网站没有在 Firefox 上进行测试，结果会导致网站在 Firefox 上停止工作。Firefox 预计会在 ESR 140 前完全移除该功能。<p></p>
</div>
