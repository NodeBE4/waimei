---
layout: post
title: "微软修复了一个导致 Firefox 高 CPU 占用的 Windows Defender bug"
date: 2023-04-11T10:24:56.000Z
author: Solidot
from: https://www.solidot.org/story?sid=74631
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1681208696000-->
[微软修复了一个导致 Firefox 高 CPU 占用的 Windows Defender bug](https://www.solidot.org/story?sid=74631)
------

<div>
微软释出了更新，修复了一个导致 Firefox 运行时高 CPU 占用的 Windows Defender bug。该 bug 最早是在五年前报告的，在 Firefox 运行时 Windows 10 内置的安全软件 Windows Defender MsMpEng.exe 的组件 Antimalware Service Executable 会表现出异常行为，导致了高 CPU 占用浏览器运行缓慢。上个月开发者终于找到了问题根源，MsMpEng.exe 在跟踪事件时高频呼叫了操作系统内核的 VirtualProtect 功能。Firefox 在生成大量事件的同时  MsMpEng.exe 执行了大量无用的计算，两者的组合导致了高 CPU 占用，Moziila 和微软合作解决了这个问题，补丁于 4 月 4 日释出，Firefox 的 CPU 占用减少了四分之三。微软同时向 Windows 7 和  Windows 8.1 推送了更新，Firefox 将一直支持这两个操作系统到 2024 年。<p></p>
</div>
