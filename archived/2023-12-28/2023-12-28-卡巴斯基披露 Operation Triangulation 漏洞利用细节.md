---
layout: post
title: "卡巴斯基披露 Operation Triangulation 漏洞利用细节"
date: 2023-12-28T07:09:47.000Z
author: Solidot
from: https://www.solidot.org/story?sid=76998
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1703747387000-->
[卡巴斯基披露 Operation Triangulation 漏洞利用细节](https://www.solidot.org/story?sid=76998)
------

<div>
今年上半年，俄罗斯安全公司卡巴斯基披露其数十名雇员遭遇网络攻击，该攻击利用 iOS 无点击漏洞在雇员的 iPhone 手机上植入恶意程序，收集麦克风录音、照片、地理位置等数据。卡巴斯基认为它不是攻击的主要目标。俄罗斯官员认为这次攻击是 NSA 发起的，有数千部外交人员的 iPhone 感染了恶意程序，尤其是位于北约、前苏联加盟国、以色列和中国等地的外交使团成员。卡巴斯基将这次行动命名为 Operation Triangulation。本周三举行的 37C3（37th Chaos Communication Congress）会议上，该公司的研究人员披露了 Operation Triangulation 的细节。该攻击利用了 4 个 0day 漏洞，适用于 iOS 16.2 以下版本。攻击者首先发送了恶意  iMessage 附件，应用在处理附件时不会向用户显示任何痕迹；恶意附件利用了无文件记录的 ADJUST TrueType 字体指令中的远程代码执行漏洞 CVE-2023-41990，该漏洞可追溯到 1990 年代。攻击者还利用了两个内核漏洞和一个浏览器漏洞。安全研究人员称，这是他们见过最复杂的攻击链。漏洞不简单，其中包括外界不知道的硬件功能。俄罗斯官员指控苹果在这次攻击行动中与 NSA 合作，从漏洞利用上看要么攻击者入侵了苹果获取了内部硬件文件，要么确实苹果与攻击者有合作。苹果否认了与 NSA 合作的指控。<p></p>
</div>
