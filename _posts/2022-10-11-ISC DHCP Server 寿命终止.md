---
layout: post
title: "ISC DHCP Server 寿命终止"
date: 2022-10-11T08:36:21.000Z
author: Solidot
from: https://www.solidot.org/story?sid=73020
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1665477381000-->
[ISC DHCP Server 寿命终止](https://www.solidot.org/story?sid=73020)
------

<div>
上周发布的 ISC DHCP v4.4.3-P1 和 4.1-ESV-R16-P2 将是最后一个维护版本，除非发现非常严重的安全漏洞，<a href="https://www.isc.org/blogs/isc-dhcp-eol/" target="_blank">ISC 没有计划继续发布更新</a>。项目的代码库将<a href="https://gitlab.isc.org/isc-projects/dhcp">停止维护</a>，用户仍然可以递交补丁和问题，但没人再去解决问题或发布补丁了。ISC DHCP 或 <a href="https://en.wikipedia.org/wiki/DHCPD">dhcpd </a>是动态主机设置协议（DHCP）的服务器程序，至今有 23 年历史，ISC 结束这个项目是因为它不是为可测试性设计的，修改代码的风险性非常高，因此过去几年它越来越少的修改代码，它创造了名叫 <a href="https://www.isc.org/kea/">Kea</a> 的新 DHCP 服务器程序，并建议使用旧版本的用户切换到该版本或其它<a href="https://en.wikipedia.org/wiki/Comparison_of_DHCP_server_software">替代</a>。
</div>
