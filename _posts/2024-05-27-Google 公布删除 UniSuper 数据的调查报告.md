---
layout: post
title: "Google 公布删除 UniSuper 数据的调查报告"
date: 2024-05-27T06:25:54.000Z
author: Solidot
from: https://www.solidot.org/story?sid=78274
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1716791154000-->
[Google 公布删除 UniSuper 数据的调查报告](https://www.solidot.org/story?sid=78274)
------

<div>
本月初，Google Cloud 云服务不小心删除了其大客户澳大利亚退休基金管理公司 UniSuper 的全部数据，幸运的是 UniSuper 在另一家公司有备份，因此这起事故没有给它造成毁灭性打击。Google 上周披露了这起事故的更多细节。UniSuper 使用了 Google Cloud VMware Engine(GCVE)服务。2023 年初，Google 的操作人员使用一个内部工具为 UniSuper 部署了 GCVE 私有云以满足特定的容量要求。该工具已被弃用，到 2023 年第四季度将完全自动化，不再需要人工操作干预。但在配置 GCVE 私有云时它意外的将一个输入参数留空。对于留空的参数，系统会自动分配一个默认的 1 年期限值。当一年期限结束后系统会删除 UniSuper 的私有云。由于删除是参数留空触发的，而不是客户要求删除，因此客户没有收到删除通知。客户发起的删除会收到通知。Google 表示已采取多项措施确保此类事故不会再次发生，包括相关内部工具已被弃用，修改了删除客户私有云的系统行为。<p></p>
</div>
