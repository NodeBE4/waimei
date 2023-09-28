---
layout: post
title: "Linux 应用 Free Download Manager 秘密植入后门三年之久"
date: 2023-09-13T15:04:28.000Z
author: Solidot
from: https://www.solidot.org/story?sid=76076
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1694617468000-->
[Linux 应用 Free Download Manager 秘密植入后门三年之久](https://www.solidot.org/story?sid=76076)
------

<div>
卡巴斯基研究人员披露了一个秘密植入后门三年之久的 Linux 应用 Free Download Manager。网站  freedownloadmanager[.]org 向 Linux 用户提供应用 Free Download Manager，但从 2020 年开始，该域名会不定时的将用户重定向到另一个域名 deb.fdmpkg[.]org 下载恶意版本。恶意版本包含了脚本会下载两个可执行文件到 /var/tmp/crond 和 /var/tmp/bs 中，脚本然后使用 cron 定时任务调度器每 10 分钟执行一次 /var/tmp/crond 中的文件，这意味着设备被永久植入了后门。安全研究人员发现，攻击者会收集系统信息、浏览历史、保存的密码、加密钱包文件以及云服务（AWS、Google Cloud、Oracle Cloud Infrastructure 和 Azure）凭证等数据，将窃取的数据上传到其控制的服务器。恶意域名的重定向在 2022 年结束，该行动目前处于不活跃状态。<p></p>
</div>
