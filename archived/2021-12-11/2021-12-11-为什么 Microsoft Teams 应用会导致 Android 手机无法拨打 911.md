---
layout: post
title: "为什么 Microsoft Teams 应用会导致 Android 手机无法拨打 911"
date: 2021-12-11T15:59:06.000Z
author: Solidot
from: https://www.solidot.org/story?sid=69970
tags: [ Solidot ]
categories: [ Solidot ]
---
<!--1639238346000-->
[为什么 Microsoft Teams 应用会导致 Android 手机无法拨打 911](https://www.solidot.org/story?sid=69970)
------

<div>
一位 Google Pixel 3 用户在祖母疑似中风时尝试拨打紧急救助电话 911 结果在铃声响了一下之后就卡死了。幸好家里还有固话，因此最后没有发生更糟糕的情况。问题被发现是安装之后没有登录的微软协作工具 Teams 应用导致的。对 Android 源代码的分析<a href="https://medium.com/@mmrahman123/how-a-bug-in-android-and-microsoft-teams-could-have-caused-this-users-911-call-to-fail-6525f9ba5e63">揭示了背后真正的原因</a>。在 Android 源代码中，名叫 adjustAttemptsforEmergency 的方法决定了哪一个 PhoneAccount 实例处理紧急呼叫。Microsoft Teams 应用使用 Skype 后端进行语音呼叫，它注册了带有 CAPABILITY_SELF_MANAGED 标记的 PhoneAccount，但它不能处理紧急呼叫，因此没有注册 CAPABILITY_PLACE_EMERGENCY_CALLS 标记。问题是 adjustAttemptsforEmergency 包含了所有的 PhoneAccount 实例列表，即使实例没有 CAPABILITY_PLACE_EMERGENCY_CALLS 标记。Teams 应用本来不应该包含在内的。但这并非是问题根源，否则每一部安装了 Teams 应用的 Android 手机都会无法拨打 911。问题的根源是在特定条件下，sortSimPhoneAccountsforEmergency 方法中的代码会导致整数溢出/下溢错误。该方法被用于对  PhoneAccount 列表进行分类，比较哪个 PhoneAccount 有紧急呼叫 CAPABILITY_PLACE_EMERGENCY_CALLS 标记，哪个是用户首选账号。如果比较的两个 PhoneAccount 实例是相同的，它会对比哈希值，因为相同的实例也会有不同的哈希值。问题是 account1.hashCode() — account2.hashCode() 的值如果小于 Integer.MIN_VALUE 或大于 Integer.MAX_VALUE 就会导致溢出。该方法通常不需要用到，因此出现整数溢出的几率是非常低的。真正的问题在于 Microsoft Teams 应用在安装之后如果没有登录，它在每一次手机冷启动之后会创造一个 PhoneAccount 实例。版本号 v1416/1.0.0.2021163901 和 1416/1.0.0.2021183702 都存在这一行为。
</div>
