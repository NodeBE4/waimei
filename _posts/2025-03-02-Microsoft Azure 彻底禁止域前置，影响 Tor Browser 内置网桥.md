---
layout: post
title: "Microsoft Azure 彻底禁止域前置，影响 Tor Browser 内置网桥"
date: 2025-03-02T10:17:23.000Z
author: Solidot
from: https://www.solidot.org/story?sid=80692
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1740910643000-->
[Microsoft Azure 彻底禁止域前置，影响 Tor Browser 内置网桥](https://www.solidot.org/story?sid=80692)
------

<div>
Gundaz Aghayev 写道:<i>微软在 4 年前宣布他们对域前置的反对立场，声称“作为一家致力于为善提供技术的公司…支持支持自由和开放沟通的某些用例是一个重要的考虑因素。然而域前置也受到从事非法活动的不良行为者和威胁行为者的滥用…在某些情况下，不良行为者会配置他们的 Azure 服务来实现这一点…我们正在改变我们的政策，以确保在 Azure 中停止和阻止域前置。”<br>在多次通知和警告之后，达摩克利斯之剑终于落下。微软去年底通知用户，旧的 Azure CDN 将于 2025 年 1 月 15 日终止，建议用户迁移到类似 Azure Front Door 服务。在新 的Azure Front Door 服务下，用户只能得到唯一的专有域名，如 snowflake-broker-hadmaqbnc4dmcffs.z03.azurefd.net，有效地阻止了利用域前置的可能性。<br>本年 2 月 1 日，Azure CDN彻底停止工作。<br>Tor Project 在 3 周前从源代码库删除内置的 meek-azure 网桥，它被另一个 CDN77 上的 meek 网桥替代。</i><p></p>
</div>
