---
layout: post
title: "Google 用 Topics 替换 FLoC"
date: 2022-01-26T05:40:22.000Z
author: Solidot
from: https://www.solidot.org/story?sid=70509
tags: [ Solidot ]
categories: [ Solidot ]
---
<!--1643175622000-->
[Google 用 Topics 替换 FLoC](https://www.solidot.org/story?sid=70509)
------

<div>
Google 去年<a href="https://www.solidot.org/story?sid=68028">宣布</a>了 Cookies 替代 Federated Learning of Cohorts (FLoC)，设计根据用户群而不是个别用户的兴趣展示广告，FLoC 引发了很多争议，多家基于 Chromium 的浏览器开发商都决定禁用 FLoC。现在 Google 决定放弃 FLoC，<a href="https://yro.slashdot.org/story/22/01/25/1519222/google-kills-off-floc-replaces-it-with-topics">提出了</a>另一个 Cookies 替代 <a href="https://github.com/jkarlin/topics">Topics API</a>。新的 API 仍然是基于用户兴趣，它通过保留过去三周的浏览历史数据评估用户的兴趣，目前 Google 将兴趣主题的数量限制在 300 个，考虑以后增加数量。Google 根据 300 个主题对用户访问的网站进行分类，以前未分类的网站将使用浏览器内置的轻量级机器学习算法根据域名提供一个主题。当用户访问支持 Topics API 的网站，浏览器将向网站分享你感兴趣的三个主题——过去三周每周一个，从排在前五的兴趣主题随机选择。网站可以与广告商分享这些信息，决定如何展示定向广告。Google 表示主题不会包含敏感类别，如性别或种族，用户还可以检查并删除主题，可以禁用 Topics API。
</div>
