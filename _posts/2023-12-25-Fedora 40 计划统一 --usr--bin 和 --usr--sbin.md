---
layout: post
title: "Fedora 40 计划统一 /usr/bin 和 /usr/sbin"
date: 2023-12-25T09:46:45.000Z
author: Solidot
from: https://www.solidot.org/story?sid=76971
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1703497605000-->
[Fedora 40 计划统一 /usr/bin 和 /usr/sbin](https://www.solidot.org/story?sid=76971)
------

<div>
在几年前合并了 /bin 和 /usr/bin 之后，Fedora 开发者提议在 Fedora 40 中统一 /usr/bin 和 /usr/sbin。理由是此举有助于简化打包者的工作和终端用户的使用，进一步兼容主流 Linux 发行版。开发者称，Fedora有 /sbin/ip，而 Debian 有 /bin/ip；Fedora 有 /bin/chmem 和 /bin/isosize，Debian 有 /sbin/chmem 和 /sbin/isosize；Fedora 有 /sbin/{addpart,delpart,lnstat,nstat,partx,ping,rdma,resizepart,ss,udevadm,update-alternatives}，而 Debian 在 /bin 下有相同的。发行版 Arch 在几年前进行了合并，此举也将让 Fedora 和 Arch 更加兼容。<p></p>
</div>
