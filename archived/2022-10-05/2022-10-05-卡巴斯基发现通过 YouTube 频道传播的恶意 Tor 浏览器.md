---
layout: post
title: "卡巴斯基发现通过 YouTube 频道传播的恶意 Tor 浏览器"
date: 2022-10-05T16:01:15.000Z
author: Solidot
from: https://www.solidot.org/story?sid=72968
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1664985675000-->
[卡巴斯基发现通过 YouTube 频道传播的恶意 Tor 浏览器](https://www.solidot.org/story?sid=72968)
------

<div>
卡巴斯基安全研究人员<a href="https://securelist.com/onionpoison-infected-tor-browser-installer-youtube/107627/" target="_blank">发现通过流行 YouTube 中文频道传播的恶意 Tor 浏览器</a>。该频道的订阅者逾 18 万，相关视频的浏览量超过 6.4 万次，视频是在 2022 年 1 月上传的，卡巴斯基的调查显示最早的受害者是在 2022 年 3 月出现的。安全研究人员将此次攻击命名为 OnionPoison，恶意版本的 Tor 浏览器为 torbrowser-install-win64-11.0.3_zh-cn.exe，没有数字签名，安装程序用 Visual Studio 2003–7.10 SDK 编译，其隐私设置比原版更弱，捆绑了恶意组件 freebl3.dll，原版也有该文件但恶意版已完全不同，浏览器禁用了更新以防止恶意版的 freebl3.dll 被覆盖。freebl3.dll 会向 C2 服务器发送请求，C2 会判断 IP 地址位置，如果在某个特定区域则会下载后续恶意负荷 cloud.dll 去收集更多信息。收集的信息包括安装软件、运行进程、Tor 浏览器历史、Google Chrome 和 Edge 浏览器历史，微信和 QQ ID，Wi-Fi 网络的 SSID 和 MAC，等等。
</div>
