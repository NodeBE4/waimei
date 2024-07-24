---
layout: post
title: "Telegram Android 版本发现 0day 漏洞允许将恶意文件伪装成视频"
date: 2024-07-23T13:54:57.000Z
author: Solidot
from: https://www.solidot.org/story?sid=78779
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1721742897000-->
[Telegram Android 版本发现 0day 漏洞允许将恶意文件伪装成视频](https://www.solidot.org/story?sid=78779)
------

<div>
安全公司 ESET 上月初在一个黑客论坛发现有人在出售一个 Android 版本的 Telegram 漏洞，允许攻击者在 Telegram 频道、群组和聊天中发送伪装成视频的恶意文件。研究人员称该漏洞为 EvilVideo，Telegram 在本月初的 v10.14.5+ 版本中修复了该漏洞。攻击者有大约五周时间利用该 0day 漏洞，但不清楚是否被利用。EvilVideo 利用了 Telegram 自动下载媒体文件的默认设置。该设置可手动禁用，但如果用户点击共享文件的下载按钮，有效负荷仍可以安装在设备上。如果用户尝试播放，Telegram 会显示无法播放的信息，建议使用外部播放器，黑客将恶意应用伪装成外部播放器。修复后的 Telegram 能正确将恶意文件识别为应用而不是视频。<p></p>
</div>
