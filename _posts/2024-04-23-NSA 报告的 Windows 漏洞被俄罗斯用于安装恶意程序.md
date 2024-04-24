---
layout: post
title: "NSA 报告的 Windows 漏洞被俄罗斯用于安装恶意程序"
date: 2024-04-23T13:48:04.000Z
author: Solidot
from: https://www.solidot.org/story?sid=77983
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1713880084000-->
[NSA 报告的 Windows 漏洞被俄罗斯用于安装恶意程序](https://www.solidot.org/story?sid=77983)
------

<div>
微软周一披露，一个高危漏洞被俄罗斯黑客组织利用了四年之久。该漏洞编号为 CVE-2022-38028，位于 Windows 打印后台处理程序中，威胁评分 7.8/10，它能与其它漏洞组合利用提权获得系统权限。该漏洞是 NSA 报告的，微软在 2022 年修复时没有披露该漏洞正被利用。周一微软披露黑客组织 Forest Blizzard 至少从 2020 年 6 月甚至可能早在 2019 年 4 月起就利用该漏洞。Forest Blizzard 的其它名字包括了 APT28、Sednit、Sofacy、GRU Unit 26165 和 Fancy Bear，被认为与俄罗斯军事情报总局的 26165 部队有关联。黑客利用漏洞获得系统权限之后会安装恶意程序 GooseEgg，该工具为后续行动提供了一个简单的界面用于安装其它具有系统权限的恶意程序。GooseEgg 会将恶意程序安装到特定子目录下，这些子目录名字包括了 Microsoft、Adobe、Comms、Intel、Kaspersky Lab、Bitdefender、ESET、NVIDIA、UbiSoft、Steam。举例来说，它可能会创建特定的目录如 C:\ProgramData\Adobe\v2.116.4405。<p></p>
</div>
