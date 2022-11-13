---
layout: post
title: "幽灵必须死：漏洞利用幽灵'msg_msg'以及VED的防护策略"
date: 2022-11-13T14:23:58.000Z
author: Solidot
from: https://www.solidot.org/story?sid=73351
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1668349438000-->
[幽灵必须死：漏洞利用幽灵'msg_msg'以及VED的防护策略](https://www.solidot.org/story?sid=73351)
------

<div>
<p><i>这两个缓解措施均是可被绕过的，VED 目前的版本是基于 LKRG 实现的，检查的完整性与性能的平衡是需要考虑的。更加严密的 msg 是可能的，但是 kprobe 的检查点数量，计算量需要多的多。另外则是虽然这两个缓解措施均可被绕过，但是叠加两者，由于其中的检查是相互交叉的，比方说完整性检查包含的 struct msg_msgseg *next, size_t m_ts，和越界检查。这使得漏洞利用需要依赖于原代码路径来实现堆喷，和更依赖同类型的 object 之间的污染，使得 msg 的漏洞利用困难程度上升。当然这些专门的绕过对资深的内核黑客来说不会是多大的问题。VED 也在探索更加完整并且平衡性能损耗的方案。"<a href='/story?sid=73351'>查看全文</a></p>
</div>
