---
layout: post
title: "韩国黑客利用 WPS Office 0day 部署恶意程序"
date: 2024-08-29T06:53:54.000Z
author: Solidot
from: https://www.solidot.org/story?sid=79106
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1724914434000-->
[韩国黑客利用 WPS Office 0day 部署恶意程序](https://www.solidot.org/story?sid=79106)
------

<div>
韩国黑客组织 APT-C-60 利用了 Windows 版 WPS Office 的一个 0day 在目标设备上安装后门 SpyGlace。WPS 是金山开发的办公软件，在全球有逾 5 亿活跃用户。黑客利用的 0day 被称为 CVE-2024-7262，影响版本从 12.2.0.13110（2023 年 8 月）到 12.1.0.16412（2024 年 3 月）。金山在 3 月悄悄修复了漏洞，但没有向客户披露该漏洞正被活跃利用，促使安全公司 ESET 就该漏洞公布了一份详细报告。CVE-2024-7262 与软件如何处理自定义协议处理器的方式相关，其中 ksoqing:// 允许文档中嵌入的特制 URL 执行外部应用。APT-C-60 创建了 MHTML 文件，嵌入了隐藏在诱饵图像下的恶意超链接，引诱受害者点击图像触发漏洞。金山修复 CVE-2024-7262 的补丁并不完整，ESET 研究人员发现了第二个任意代码执行的高危漏洞 CVE-2024-7263。金山在 5 月修复了新的漏洞。为修复这两个漏洞 WPS 用户需要尽可能快的升级到 v12.2.0.17119 及以上版本。<p></p>
</div>
