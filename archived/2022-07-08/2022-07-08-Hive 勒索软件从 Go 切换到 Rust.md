---
layout: post
title: "Hive 勒索软件从 Go 切换到 Rust"
date: 2022-07-08T10:25:00.000Z
author: Solidot
from: https://www.solidot.org/story?sid=72068
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1657275900000-->
[Hive 勒索软件从 Go 切换到 Rust](https://www.solidot.org/story?sid=72068)
------

<div>
微软安全研究人员<a href="https://www.zdnet.com/article/this-ransomware-just-switched-programming-languages-from-go-to-rust-heres-why/">发现</a>，一年前用 Go 语言编写的 Hive 勒索软件有了用 Rust 重写的新变种。Hive 于 2021&nbsp; 年 6 月出现，两个月后 FBI 对此发出<a href="https://www.ic3.gov/Media/News/2021/210825.pdf">警告</a>。11 月，欧洲电子零售巨头 MediaMarkt 受到了 Hive 的攻击。这是另一个勒索软件即服务(RaaS)双重勒索团伙，该团伙最近一直在针对存在漏洞的 Microsoft Exchange 服务器和 RDP 服务器、窃取的 VPN 凭据和网络钓鱼部署勒索软件并窃取值得窃取的信息。Hive 迁移到 Rust 版本已进行了几个月，它吸取了 BlackCat 勒索软件的教训，后者也是用 Rust 编写的。Group-IB 研究人员在 3 月发现 Hive 将其 Linux 加密器（针对 VMware ESXi 服务器）转换为 Rust，让安全研究人员更难以窥看其与受害者的赎金对话。微软的分析表明，用 Rust 重写的 Hive 更加全面，支持在 3 月份提到的对加密方法的更改。微软指出，“它不是在加密的每个文件中嵌入一个加密密钥，而是在内存中生成两组密钥，用它们加密文件，然后将两组密钥加密并写入它所加密的驱动器的根目录，两者都使用 .key 扩展名。”
</div>
