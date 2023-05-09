---
layout: post
title: "当 Windows 用户在恐慌下删除 system32\curl.exe"
date: 2023-04-24T13:47:27.000Z
author: Solidot
from: https://www.solidot.org/story?sid=74771
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1682344047000-->
[当 Windows 用户在恐慌下删除 system32\curl.exe](https://www.solidot.org/story?sid=74771)
------

<div>
curl 作者 Daniel Stenberg 说，Windows 10 和 11 自带的 curl 工具包含了一个低危漏洞，该漏洞已经修复了，微软也释出了补丁，但补丁释出前部分用户自行删除了存在漏洞的版本，导致无法更新，他表示 curl 项目对此不负任何责任，有问题找微软。<i>Windows 10 和 11 操作系统包含的 curl 工具位于 System32 系统文件夹下，这里面的程序是不能随便删除或替换的。2022 年 12 月 curl 项目报告了一个释放后使用（Use-After-Free）的低危漏洞 CVE-2022-43552，但美国国家漏洞数据库可能是为了督促用户尽快更新而提高了该漏洞的危险等级，将其列为中危漏洞。导致的结果是 2022 年 12 月 21 日之后的某个时间安全扫描工具开始就系统中包含存在漏洞的工具对用户发出警告。这让部分用户恐慌了。他们删除或替换了 C:\Windows\System32\curl.exe。微软在 4 月 11 日的例行安全更新中修复了该漏洞释出了补丁 KB5025221，但那些自行删除系统文件的用户发现 Windows 更新程序拒绝更新。Stenberg 表示 curl 项目对此无能为力。</i><p></p>
</div>
