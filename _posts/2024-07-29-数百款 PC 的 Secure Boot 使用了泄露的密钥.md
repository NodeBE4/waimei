---
layout: post
title: "数百款 PC 的 Secure Boot 使用了泄露的密钥"
date: 2024-07-29T08:05:53.000Z
author: Solidot
from: https://www.solidot.org/story?sid=78823
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1722240353000-->
[数百款 PC 的 Secure Boot 使用了泄露的密钥](https://www.solidot.org/story?sid=78823)
------

<div>
2007 年，中国研究员 icelord 在 CSDN 发表了一篇博文，介绍了 BIOS Rootkit 的一种简单实现。2011 年，被称为 Mebromi 的 BIOS Rootkit 实现走到了现实生活里。2012 年行业联盟宣布采用 Secure Boot 去抵御 BIOS 恶意程序。Secure Boot 基于 BIOS 继任者 UEFI，它使用公钥加密阻止加载任何未使用预批准数字签名签名的代码。固件安全供应商 Binarily 上周发布的报告显示，戴尔、宏碁、富士通、技嘉、惠普、英特尔、联想和超微销售的数百款 PC 使用了 2022 年泄露的测试平台密钥(PK)保护其 UEFI Secure Boot 实现。加密密钥的泄露意味着 Secure Boot 所提供的安全保护被破坏了。泄露密钥由 AMI 创建，主要提供给客户测试用，但测试密钥却不知何故进入了产品中，而且在这些公司的 PC 产品中共享。Binarly 创始人兼 CEO Alex Matrosov 指出，想象一下，一栋公寓楼所有住客都有相同的前门锁和钥匙。如果有人丢失钥匙，整栋楼都会出问题。更糟的情况是，其它建筑物也使用了相同的锁和钥匙。总共有 215 款 PC 受到影响，你可以检查下自己使用的 PC 型号是否名单中。<p></p>
</div>
