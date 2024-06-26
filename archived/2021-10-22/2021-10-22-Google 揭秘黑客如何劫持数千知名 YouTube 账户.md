---
layout: post
title: "Google 揭秘黑客如何劫持数千知名 YouTube 账户"
date: 2021-10-22T10:00:02.000Z
author: Solidot
from: https://www.solidot.org/story?sid=69343
tags: [ Solidot ]
categories: [ Solidot ]
---
<!--1634896802000-->
[Google 揭秘黑客如何劫持数千知名 YouTube 账户](https://www.solidot.org/story?sid=69343)
------

<div>
2019 年以来，黑客一直在劫持知名的 YouTube 频道。有时他们会广播一些加密货币骗局，有时只是拍卖这些账户的访问权。现在 Google 详细<a href="https://blog.google/threat-analysis-group/phishing-campaign-targets-youtubers-cookie-theft-malware/" target="_blank">揭露了</a>这些受雇黑客过去几年用于入侵数千名 YouTube 内容作者的技术。<br><br>加密货币骗局和账户接管并不罕见；去年秋天的 Twitter 黑客事件就是一个例子。但针对 YouTube 帐户持续不断的攻击却因其广度和黑客使用的方法而引人注目。他们采用的是一种古老的策略，尽管如此，防御却非常棘手。<br><br>攻击都始于网络钓鱼。攻击者会向 YouTube 作者发送一封看似来自真实服务的电子邮件——例如 VPN、照片编辑应用程序或防病毒产品，并提出合作建议。他们提议进行标准的促销：向你的观众展示我们的产品，我们将向你支付费用。对于 YouTube 网红来说，这是每天都在发生的交易，网红借此获得收益。<br><br>然而点击链接下载产品会将他们带到恶意软件登录站点——而不是真正的交易站点。某些情况下，黑客会冒充 Cisco VPN 和 Steam 等知名网站，或者冒充专注新冠的媒体。Google 表示，它迄今发现了 1000 多个域名，这些钓鱼域名都是为感染不知情的 YouTube 用户建立的。这暗示出了此类攻击的规模。该公司还发现了 15,000 个与这些计划背后的攻击者有关的电邮账户。这些攻击者似乎并不是一伙的；Google 表示，在俄语论坛上有各种黑客都在宣传账户接管服务。<br><br>一旦 YouTube 用户下载了恶意软件，它就会从他们的浏览器中获取特定的 cookie。这些“会话 cookie”确认用户已成功登录到他们的账户。黑客可以将这些偷来的 cookie 上传到恶意服务器，让他们冒充已通过身份验证的受害者。会话 cookie 对攻击者来说特别有价值，因为它们不需要再经过登录流程的任何部分。
</div>
