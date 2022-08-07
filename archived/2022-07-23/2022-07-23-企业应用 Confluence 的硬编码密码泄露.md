---
layout: post
title: "企业应用 Confluence 的硬编码密码泄露"
date: 2022-07-23T10:30:35.000Z
author: Solidot
from: https://www.solidot.org/story?sid=72231
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1658572235000-->
[企业应用 Confluence 的硬编码密码泄露](https://www.solidot.org/story?sid=72231)
------

<div>
澳大利亚公司 Atlassian 开发的企业维基软件 Confluence 被发现有硬编码密码，更糟糕的是<a href="https://arstechnica.com/information-technology/2022/07/atlassian-warns-hardcoded-password-flaw-is-likely-to-be-exploited-in-the-wild/" target="_blank">密码还被泄露了</a>。存在硬编码的应用是 <a href="https://marketplace.atlassian.com/apps/1211644/questions-for-confluence?hosting=server&amp;tab=overview">Questions for Confluence</a>，它在安装时会创建名叫 disabledsystemuser 的账号，旨在帮助管理员在应用和  Confluence 云服务之间转移数据。Atlassian 承认未经授权的远程攻击者在知道硬编码密码之后可登陆  Confluence 访问用户组能访问的任何页面。受影响的版本是  Questions for Confluence versions 2.7.x 和 3.0.x。用户可搜索是否存在 User: disabledsystemuser，Username: disabledsystemuser 和 Email: dontdeletethisuser@email.com。
</div>
