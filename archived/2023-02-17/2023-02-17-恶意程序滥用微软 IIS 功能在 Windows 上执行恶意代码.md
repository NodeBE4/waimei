---
layout: post
title: "恶意程序滥用微软 IIS 功能在 Windows 上执行恶意代码"
date: 2023-02-17T10:12:06.000Z
author: Solidot
from: https://www.solidot.org/story?sid=74164
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1676628726000-->
[恶意程序滥用微软 IIS 功能在 Windows 上执行恶意代码](https://www.solidot.org/story?sid=74164)
------

<div>
安全公司赛门铁克的研究人员发现一种恶意程序滥用微软 IIS 的一项功能隐蔽的渗出数据和执行恶意代码。微软 IIS（Internet Information Services）是广泛使用的 Web 服务器，它的一项功能叫 Failed Request Event Buffering（FREB），旨在帮助管理员诊断错误，FREB 能从缓存中将部分错误相关的请求写入磁盘。黑客找到了滥用该功能的方法，攻击者首先需要入侵运行 IIS 的 Windows 系统，启用 FREB，通过将恶意代码注入 IIS 进程内存劫持执行，它随后就能拦截所有 HTTP 请求，寻找特殊格式的请求，这种特殊的请求能以隐蔽的方式执行远程代码，系统上没有可疑文件或进程在运行。研究人员将这种恶意程序命名为 Frebniis。<p></p>
</div>
