---
layout: post
title: "Intel Alder Lake固件整体方案泄漏分析"
date: 2022-10-09T03:01:44.000Z
author: Solidot
from: https://www.solidot.org/story?sid=72989
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1665284504000-->
[Intel Alder Lake固件整体方案泄漏分析](https://www.solidot.org/story?sid=72989)
------

<div>
<a href="http://https://hardenedvault.net/">HardenedVault</a> 写道 "<i>这次泄漏的主角是固件供应商Insyde的部分开发框架，其框架集成了Intel授权的内容，这个框架主要是为其客户OEM厂商Lenovo（联想）服务，根据<a href="https://github.com/LCFCASD/ICE_TEA_BIOS">github泄漏仓库</a>的时间戳信息，2022年9月30日，一名未确认身份的用户上传了Intel Alder Lake平台的固件整体方案，其中包含参考实现，OEM实现，IBV方案以及相关文档，大小为4.8GB。2022年10月8日，此次泄漏引起了<a href="https://www.tomshardware.com/news/intels-alder-lake-bios-source-code-reportedly-leaked-online">媒体tom’sHardware的关注和报道</a>，随后<a href="https://hardenedvault.net/zh-cn/blog/2022-10-08-alderlake_fw-leak/" target="_blank">泄漏仓库被删除</a>，但安全研究者依然可以<a href="https://hardenedvault.net/zh-cn/blog/2022-10-08-alderlake_fw-leak/" target="_blank">时间机器获得泄漏内容</a>。Insyde作为固件整体方案商会持续开发和集成各平台的支持，此次泄漏的内容是Insyde方案的删减版本，仅支持Alder Lake，泄漏的内容有几个比较有趣的内容：<ul><li>由Insyde提供的完整工具链，用于简化<a href="https://hardenedvault.net/zh-cn/blog/2022-10-08-alderlake_fw-leak/" target="_blank">OEM厂商的开箱以及BIOS镜像调整工</a>作</li><li>Insyde的定制框架，其封装了兼容EDK2的接口，让ODM/OEM厂商更容易集成平台组件比如Intel FSP</li><li><a href="https://hardenedvault.net/zh-cn/blog/2022-10-08-alderlake_fw-leak/" target="_blank">Intel参考实现以及OEM的实现</a>，这次泄露事件中的OEM主角是Lenovo联想</li><li>Binary blobs：值得注意的是，其中除了各种设备（蓝牙BLE，WiFi，以太网等）所需要的binary blobs外，也包含了三种不同的用于安全特性的ACM：BiosGuard，BootGuard以及TXT</li><li>另外，一个值得关注的点是<a href="https://hardenedvault.net/zh-cn/blog/2022-10-08-alderlake_fw-leak/" target="_blank">BootGuard开箱所用的密钥堆</a>也在泄漏内容中，x86启动的前半部的ACM是由Intel签名，后半部则是OEM厂商控制，让我们祈祷Lenovo并没有将它们用于生产环境，请证明我们是错的！"</li></ul></i>
</div>
