---
layout: post
title: "Firefox 如何改进 macOS 版本的响应"
date: 2022-10-11T14:08:20.000Z
author: Solidot
from: https://www.solidot.org/story?sid=73023
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1665497300000-->
[Firefox 如何改进 macOS 版本的响应](https://www.solidot.org/story?sid=73023)
------

<div>
macOS 用户可能注意到 Firefox v103 版本的响应<a href="https://hacks.mozilla.org/2022/10/improving-firefox-responsiveness-on-macos/" target="_blank">有了显著改进</a>，尤其是在打开大量标签的情况下。Firefox 的内存分配器在 macOS 平台依赖于系统自带的 <a href="https://developer.apple.com/library/archive/documentation/System/Conceptual/ManPages_iPhoneOS/man3/spinlock.3.html" target="_blank">OSSpinLock</a> 去执行自旋锁(spin lock)和互斥量(mutex)功能。但 OSSpinLock 的自旋锁存在基础性缺陷，它是在用户空间内执行的，用户空间并不知系统负载信息，如果是在内核空间则能根据负载做出合理决策，用户空间锁则可能在系统高负载的情况下执行自旋锁结果增加了额外负载。苹果知道 OSSpinLock 的问题，它提供了 <a href="https://developer.apple.com/documentation/os/os_unfair_lock" target="_blank">os_unfair_lock</a> 作为 OSSpinLock 的官方替代。但开发者在测试后发现 os_unfair_lock 反而会导致性能下降，进一步分析发现 os_unfair_lock 支持内核空间锁，但并没有在文档中记录下来。在启用了 os_unfair_lock 的内核空间自适应自旋锁之后，Firefox 的响应有了显著改进。该功能需要 macOS 10.15 及以上版本才能支持。
</div>
