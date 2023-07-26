---
layout: post
title: "AMD Zen 2 架构处理器曝出 Zenbleed 预测漏洞"
date: 2023-07-26T09:09:07.000Z
author: Solidot
from: https://www.solidot.org/story?sid=75620
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1690362547000-->
[AMD Zen 2 架构处理器曝出 Zenbleed 预测漏洞](https://www.solidot.org/story?sid=75620)
------

<div>
Google Project Zero 安全团队的 Tavis Ormandy 披露了 AMD Zen 2 架构处理器的 Zenbleed 漏洞(CVE-2023-20593)。该漏洞影响基于 Zen 2 的消费级、工作站和服务器处理器。漏洞允许攻击者从 CPU 寄存器窃取数据。现代处理器利用预测执行机制通过预测下一步的任务加速操作，Zen 2 处理器无法从特定类型的预测错误中正确恢复， Zenbleed 能利用该漏洞窃取敏感数据。它会导致 CPU 以每秒最高 30 KB 的速度泄露数据，其中包括加密密钥、root 和用户密码等敏感信息。该漏洞能被远程利用，恶意网站可通过加载 JS 触发。好消息是目前还没有观察到漏洞利用，但随着 Zenbleed 的披露情况可能会发生改变。修复该漏洞的微码已经释出，未更新的 Linux 用户需要尽快更新。<p></p>
</div>
