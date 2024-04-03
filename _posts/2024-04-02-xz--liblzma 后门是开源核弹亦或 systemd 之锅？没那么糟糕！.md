---
layout: post
title: "xz/liblzma 后门是开源核弹亦或 systemd 之锅？没那么糟糕！"
date: 2024-04-02T15:39:57.000Z
author: Solidot
from: https://www.solidot.org/story?sid=77766
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1712072397000-->
[xz/liblzma 后门是开源核弹亦或 systemd 之锅？没那么糟糕！](https://www.solidot.org/story?sid=77766)
------

<div>
Shawn the R0ck 写道：2024年3月29日，一份关于在自由软件社区备受争议的开源项目 xz 软件包被上游源代码中的后门所污染的报告在 oss-security 邮件列表中曝光。这个后门影响到了 liblzma 库，它是 xz 软件包的一部分，在第一份报告发布后有多了很多跟进的研究，内容主要如下，1） 这个后门完整地存在于发布的 xz 源码包中(5.6.0 和 5.6.1 版本)，但上游 git 仓库中存在伪装为测试数据，但并未插入 liblzma 中的载荷，而打包前单独加入源码包中的唤醒代码（它们不存在于 git 仓库中，因此从 git 仓库，或由 github 生成的源码包编译的 liblzma 中不会有后门）会将载荷注入到构建过程中。2） 注入的代码修改 Makefile 以包含恶意文件，这些文件在构建过程中被执行,导致进一步的有效载荷注入。3） 这个有效载荷针对的是使用 gcc 和 GNU 链接器的 x86-64 GNU/Linux 系统,并且是 Debian 或 RPM 软件包构建的一部分。4） 恶意代码针对 OpenSSH 服务器进行劫持以实现远程代码执行，但显著降低了登录速度。它通过劫持和修改 liblzma 库中的某些函数来实现这一点，其载荷是间接加载到 sshd 中的。sshd 实现了对 systemd-notify 的支持，liblzma 被加载是因为它是 libsystemd 的其他部分所依赖的，systemd 的复杂度再次成为了实际上的安全隐患。5） 建议立即升级任何可能受影响的系统，因为这些被污染的版本还未广泛被 GNU/Linux 发行版集成。6） 提供了一个脚本来检测系统是否可能受到影响。7）后门投毒者关闭了 LANDLOCK 沙箱，这个已经被主要维护者修复。开源社区诸多用户都对于 systemd 饱受争议的复杂性以及其生态渗透到 GNU/Linux 系统之深本有意见，借愚人节之机满足读者的阴谋论叙事的诉求：幕后黑手其实是 M$，意在摧毁 GNU/Linux 生态，首先，他们秘密收买了 Lennart Poettering，让他开发了 systemd。Lennart 在 M$ 的授意下,将 systemd 逐步渗透到 GNU/Linux 发行版中,为后续行动铺路，2022年3月，M$ 认为可以执行下一步计划了就排出了 Jia Tan 团队跟 xz-utils 社区进行交涉，Lennart Poettering 的任务也宣告结束，2022年6月，M$ 公开召回（雇佣）Lennart，此后 M$ 筹划了 2023 年开始支持 openssh 的 systemd 生态进而让 Jia TAN 去掌控整个 GNU/Linux 生态，只是没想到被一个执着于性能且追求计算美学的工程师破坏了原本完美的计划，M$立马命令Github关闭了相关的帐号以毁灭证据，幸运的是这个蔚蓝色的星球的赛博网络里有时空穿梭机，这让github的重要信息得以保留。<p></p>
</div>
