---
layout: post
title: "Snap 前开发者开发脚本用 Flatpaks 取代 Snap"
date: 2023-07-02T15:14:06.000Z
author: Solidot
from: https://www.solidot.org/story?sid=75398
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1688310846000-->
[Snap 前开发者开发脚本用 Flatpaks 取代 Snap](https://www.solidot.org/story?sid=75398)
------

<div>
Alan Pope 在 2021 年离开了工作了 10 年的 Canonical 公司，是 Canonical 主导的包格式 Snap 的共同开发者。该公司今年早些时候发布的 Ubuntu 23.04 默认移除了对竞争对手 Flatpak 格式的支持。Flatpak 和 Snap    都类似 docker，旨在提供一种独立于发行版的打包格式，解决包依赖问题，能在不导致依赖地狱的情况下在同一个系统上安装同一个程序的多个版本。Flatpak 由 Red Hat 主导开发，完全开源，能存在多个 Flatpak 软件库。相比下，Snap 的后端是 Canonical 私有的，只存在一个 Canonical 控制的 Snap 应用商店。Alan Pope 开发了一个脚本 unsnap，如果一个 Snap 软件包存在对应的 Flatpak 包，那么它将会自动用 Flatpak 包替换 Snap 包。该脚本托管在 GitHub 上。<p></p>
</div>
