---
layout: post
title: "守护者的零之曙光：Hardened SIEM/XDR"
date: 2023-08-26T03:45:05.000Z
author: Solidot
from: https://www.solidot.org/story?sid=75901
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1693021505000-->
[守护者的零之曙光：Hardened SIEM/XDR](https://www.solidot.org/story?sid=75901)
------

<div>
Shawn the R0ck 写道：现代网络安全运营中心主要依赖于两个关键要素：基于agent的安全解决方案，在台式机、笔记本和服务器操作系统上运行；以及威胁分析系统，通常称为安全信息与事件管理（SIEM）系统或扩展检测与响应（XDR）系统充当安全大脑的角色。然而，网络安全行业面临两个主要挑战。首先，大多数安全解决方案未能在操作系统（OS）及OS以下层面提供全面的威胁检测，导致这一关键领域容易受到攻击。安全大脑本身或者周边的安全产品被攻陷并不是一件有趣的事情，安全领域最尴尬之处莫过于次。其次，威胁分析系统通常缺乏与最佳安全实践相一致的强大保护措施，这可能无意中导致安全漏洞。针对这些挑战，HardenedVault开发了一种基于开源SIEM/XDR工具Wazuh的解决方案，以展示HardenedVault可以如何解决这些问题。该工具与VED无缝集成，扩展了对Linux内核运行时的监控维度，实时监控漏洞提权、容器逃逸和rootkit，同时提供了其他安全措施，如CIS合规性，为已识别的威胁提供了强大的解决方案。VED能够将SIEM/XDR的监控维度扩展到Linux内核运行时，以应对特权升级、容器逃逸和Rootkits等安全威胁，这是一个强大的增强功能。通过整合这一功能，VED可以为内核中潜在的安全威胁提供全面的可见性和检测能力。这确保了主动防御，并增强了系统的整体安全状态，从而保护系统免受复杂的攻击和未经授权的访问尝试。目前，HardenedVault在AWS上提供了Hardened SIEM/XDR，方便集成和部署。对于那些有兴趣在自建机房环境中实施类似解决方案的用户，HardenedVault将乐意提供帮助。<p></p>
</div>
