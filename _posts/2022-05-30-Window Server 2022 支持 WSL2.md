---
layout: post
title: "Window Server 2022 支持 WSL2"
date: 2022-05-30T07:19:49.000Z
author: Solidot
from: https://www.solidot.org/story?sid=71670
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1653895189000-->
[Window Server 2022 支持 WSL2](https://www.solidot.org/story?sid=71670)
------

<div>
微软释出了 Window Server 2022 的预览补丁（可选更新，下个月自动推送）<a href="https://support.microsoft.com/en-us/topic/may-24-2022-kb5014021-os-build-20348-740-preview-2b180bd4-dceb-4c49-b8cf-402b342ebc84" target="_blank">KB5014021</a>，为该操作系统引入了对 Windows Subsystem for Linux 2（WSL2）的支持。WSL2 是在 2019 年 5 月发布的，它使用真正的 Linux 内核，第一代 WSL 只提供了等价的 Linux API，性能比原生 API 差很多，第二代使用 Hyper-V 创建一个轻量级虚拟机运行 Linux 内核。WSL2 此前只提供给了桌面版本如 Windows 10，没有提供给服务器版本 Window Server，微软的理由是 WSL2 不是为在生产场景中使用而设计的。但在用户的呼声中，微软<a href="https://linux.slashdot.org/story/22/05/28/0348246/microsoft-brings-windows-subsystem-for-linux-2-to-window-server-2022" target="_blank">最终改变了立场</a>。
</div>
