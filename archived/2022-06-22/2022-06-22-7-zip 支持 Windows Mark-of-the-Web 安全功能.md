---
layout: post
title: "7-zip 支持 Windows Mark-of-the-Web 安全功能"
date: 2022-06-22T15:57:42.000Z
author: Solidot
from: https://www.solidot.org/story?sid=71913
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1655913462000-->
[7-zip 支持 Windows Mark-of-the-Web 安全功能](https://www.solidot.org/story?sid=71913)
------

<div>
7-zip 加入了对 Windows Mark-of-the-Web 安全功能的支持。当用户从网络下载文档和可执行文件，Windows 会对其加入特定的标识符 Mark-of-the-Web，告诉操作系统和支持的应用程序，文件是从另一台计算机或网络上下载的，打开文件可能会存在安全风险。举例来说，Microsoft Office 在打开文件时会检查 Mark-of-the-Web，如果有该标识符它会在保护视图下打开文件，文件处于只读模式，禁用了宏功能。7-zip 是最流行的解压缩软件之一，其作者 Igor Pavlov 在 <a href="https://www.7-zip.org/history.txt" target="_blank" rel="nofollow noopener">7-zip 22.00</a> 中加入了一个新设置，<a href="https://www.bleepingcomputer.com/news/microsoft/7-zip-now-supports-windows-mark-of-the-web-security-feature/" target="_blank">允许用户启用</a> Mark-of-the-Web 功能。
</div>
