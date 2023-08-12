---
layout: post
title: "VED-eBPF：使用 eBPF 进行内核漏洞和 Rootkit 检测"
date: 2023-08-11T15:22:53.000Z
author: Solidot
from: https://www.solidot.org/story?sid=75777
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1691767373000-->
[VED-eBPF：使用 eBPF 进行内核漏洞和 Rootkit 检测](https://www.solidot.org/story?sid=75777)
------

<div>
Shawn the R0ck 写道：我们很高兴地介绍 VED-eBPF，这是一种创新的概念验证实现，展示了 eBPF（扩展伯克利数据包过滤器）技术在为 Linux 系统提供强大的内核安全监控和漏洞检测方面的能力。VED-eBPF 利用 eBPF 的功能，提供对内核漏洞和 Rootkit 的运行时分析和检测。开源版本使用 AGPLv3 许可证发布。<br>使用 eBPF 增强内核安全 eBPF 是一种内核中的虚拟机，可以在内核中执行代码，无需修改内核源代码。通过 VED-eBPF，我们利用 eBPF 的潜力来跟踪安全敏感的内核行为并检测可能表示恶意活动的异常情况。<br>VED-eBPF 的关键特性：<br>控制流完整性（wCFI）：VED-eBPF 包含 wCFI，专注于检测控制流劫持攻击。通过跟踪内核调用栈，VED-eBPF 生成一个有效调用位置的位图，并根据此位图验证返回地址。任何无效的返回地址（表示堆栈已被破坏）都会触发安全事件进行进一步分析。<br>特权提升检测（PSD）：VED-eBPF 集成了 PSD，用于检测未经授权的特权提升。通过监视内核中的凭证结构的变化，VED-eBPF 在特定函数调用之前和之后比较凭证，以识别任何未经授权的修改。当检测到非法特权提升时，会生成一个安全事件进行分析。<br>VED-eBPF 的工作原理 VED-eBPF 将 eBPF 程序附加到相关的内核函数，实现执行流程的跟踪和安全事件的提取。然后，这些事件将通过 perf 缓冲区提交到用户空间进行进一步分析，确保实时检测潜在威胁。<br>加入我们，探索 eBPF 的安全能力 我们邀请所有对利用 eBPF 进行安全缓解感兴趣的安全爱好者、研究人员和开发人员一起探索 VED-eBPF。通过利用 eBPF 的跟踪能力和 perf 缓冲区，VED-eBPF 展示了如何实时提取和分析关键的安全事件，以识别新出现的内核威胁。<p></p>
</div>
