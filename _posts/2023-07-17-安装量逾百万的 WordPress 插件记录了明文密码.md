---
layout: post
title: "安装量逾百万的 WordPress 插件记录了明文密码"
date: 2023-07-17T07:51:24.000Z
author: Solidot
from: https://www.solidot.org/story?sid=75532
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1689580284000-->
[安装量逾百万的 WordPress 插件记录了明文密码](https://www.solidot.org/story?sid=75532)
------

<div>
All-In-One Security（AIOS）是一款安装量逾百万的 WordPress 安全插件，三周前它被发现记录明文密码并将其存储在管理员可访问数据库中后释出了安全更新。开发者表示，用户登陆使用 AIOS 的网站后明文密码会被记录，该 bug 是在 5 月释出的 v5.1.9 中引入的，上周释出的 v5.2.0 修复了 bug 并从数据库里删除了相关数据。拥有最高全新的管理员可以访问明文密码。以明文形式储存密码是安全大忌。储存密码可接受的做法是使用哈希加密，因此即使密码数据库被恶意者窃取，他们通常会很难在短时间内暴力破解。<p></p>
</div>
