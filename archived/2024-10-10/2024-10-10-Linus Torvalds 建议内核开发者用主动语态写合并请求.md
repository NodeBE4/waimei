---
layout: post
title: "Linus Torvalds 建议内核开发者用主动语态写合并请求"
date: 2024-10-10T08:06:35.000Z
author: Solidot
from: https://www.solidot.org/story?sid=79449
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1728547595000-->
[Linus Torvalds 建议内核开发者用主动语态写合并请求](https://www.solidot.org/story?sid=79449)
------

<div>
Linux 作者 Linus Torvalds 罕见的谈论了内核开发者们的书写风格。他说自己在阅读维护者们递交的合并请求（Pull Request）时会随手处理下空格或缩进问题，但语态问题没办法随手处理，会需要额外的工作。部分内核开发者在合并请求中使用了被动语态，Linus Torvalds 建议他们使用主动语态，最好还是命令式的。他举例说，维护者应避免写类似的被动语态“In this pull request, the Xyzzy driver error handling was fixed to avoid a NULL pointer dereference.”他建议写成主动语态“This fixes a NULL pointer dereference in...”或者“Fix NULL pointer dereference in&nbsp;...”他认为主动语态更简单明了。<p></p>
</div>
