---
layout: post
title: "内核补丁将 kallsyms_lookup_name()查找速度提高 715 倍"
date: 2022-12-14T09:25:10.000Z
author: Solidot
from: https://www.solidot.org/story?sid=73648
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1671009910000-->
[内核补丁将 kallsyms_lookup_name()查找速度提高 715 倍](https://www.solidot.org/story?sid=73648)
------

<div>
Linux 6.2 合并了华为开发者 Zhen Lei 递交的一个补丁，将 kallsyms_lookup_name()的查找速度提高了 715 倍。kallsyms_lookup_name() 用于根据名字查找一个符号的地址，能用于查找内核符号表中的任何符号。Zhen Lei 此前在补丁描述中解释说，目前内核使用的查找方法是将 kallsyms_names 中的符号逐一展开，然后查找，这种算法的时间复杂度是 O(n)。如果像地址一样将名字按升序排序，可以使用二进制搜索。这种算法的时间复杂度是 O(log(n))。从 O(n) 到 O(log(n)) 查找时间可以大幅减少。<p></p>
</div>
