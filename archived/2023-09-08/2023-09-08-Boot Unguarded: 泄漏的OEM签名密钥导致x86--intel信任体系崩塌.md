---
layout: post
title: "Boot Unguarded: 泄漏的OEM签名密钥导致x86/intel信任体系崩塌"
date: 2023-09-08T01:19:21.000Z
author: Solidot
from: https://www.solidot.org/story?sid=76022
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1694135961000-->
[Boot Unguarded: 泄漏的OEM签名密钥导致x86/intel信任体系崩塌](https://www.solidot.org/story?sid=76022)
------

<div>
Shawn the R0ck 写道：2023年3月，微星国际（MSI）遭受了由Money Message勒索软件组织发起的一次重大攻击。不幸的是，这不仅仅是一次随机泄露。事后的调查揭示了内部数据的泄露，包括高度敏感的信息，如BootGuard私钥。该私钥是英特尔硬件信任和加密密钥管理系统的核心组成部分，意味着存在一个难以轻易修复的漏洞，使得特定设备型号的主要安全机制可以被绕过。此外，泄露的数据还暴露了UEFI固件镜像签名密钥，进一步加剧了这次安全漏洞的严重性。<br>BootGuard安全机制与CPU微码和CSME共同构成了英特尔核心安全机制的基础。它作为硬件信任系统中的关键完整性保护机制，而UEFI固件则是计算机系统中重要的底层软件组件。通过成功攻击漏洞（例如：CVE-2020-8705）或获取来自OEM/ODM制造商的私钥，BootGuard的被破坏使得威胁行为者可以利用UEFI实现的缺陷、配置错误和其他漏洞来绕过多个已建立的安全措施和缓解措施，例如：SMM_BWP、BWE/BLE、PRx硬件安全机制、SecureBoot以及内核安全缓解技术，如HCVI、PatchGuard、kASLR、KDEP、SMEP、SMAP。此外，主流的杀毒软件和EDR/XDR系统变得无效，使攻击者持久控制被入侵的设备。Hardcore Matrix团队经过广泛研究，重建了制造商缺失的内部工具，并成功执行了针对MSI Modern-15-B12M笔记本电脑（配备英特尔第12代CPU：i5-1235U）的全面攻击链。演示涵盖了BootGuard私钥重签名、胶囊更新重签名和SMM根套件部署等活动。这个令人信服的演示视频凸显了供应链威胁的严重性，展示了它们在现实世界中的影响。该演示不涵盖操作系统内核攻击技术或SMM启动套件，因为这些技术已经有多个开源实现进行了文档化。<br>当前，全球面临严峻形势，恶意软件/勒索软件攻击中使用引导套件的情况日益增多。微星国际泄露的OEM签名密钥进一步加剧了x86固件安全本就脆弱的状态。尽管如此，许多人（包括安全专业人员）仍然难以理解源自操作系统以下层面的威胁的重要性。考虑一下，如果引导套件被植入加密托管密钥管理服务节点的固件中，可能造成的后果。这样的攻击可以通过利用内存扫描和钩子来轻松实现弱熵作为一种服务。在这种情况下，攻击者可以通过轻微的暴力攻击从公共链中窃取私钥，而无需实际接触托管基础设施。<br>然而，没有必要因此陷入恐慌，也不明智地寄希望于像RISC-V或Rust这样的“未来技术”。相反，尝试掌控每个设备的安全供应过程是一个可行的计划。听起来像个好计划！坚持这个该死的计划！这是一个很好的起点，不是吗？<p></p>
</div>
