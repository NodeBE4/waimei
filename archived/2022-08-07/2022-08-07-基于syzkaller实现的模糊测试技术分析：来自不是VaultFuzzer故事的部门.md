---
layout: post
title: "基于syzkaller实现的模糊测试技术分析：来自不是VaultFuzzer故事的部门"
date: 2022-08-07T09:46:24.000Z
author: Solidot
from: https://www.solidot.org/story?sid=72384
tags: [ Solidot ]
comments: True
categories: [ Solidot ]
---
<!--1659865584000-->
[基于syzkaller实现的模糊测试技术分析：来自不是VaultFuzzer故事的部门](https://www.solidot.org/story?sid=72384)
------

<div>
<a href="http://https://hardenedvault.net/">HardenedVault</a> 写道<i> "2017年的晚些时候，<a href="https://hardenedvault.net/zh-cn/blog/2022-08-07-state-based-fuzzer-update/" target="_blank">一名匿名黑客建议HardenedLinux</a>可以尝试把语料库和特定的代码路径形成具备概率性的关联，经过HardenedLinux maintiner的内部讨论认为syzkaller作为通用框架对于大规模QA的生产环境仍有大量的改进空间，假设GCP的工程师也是如此思路的话，那的确可以完成更全面的QA工程化。2018年，HardenedLinux的maintainer尝试使用eBPF在函数入口和出口收集一些函数接口中的结构体及其数值，即便这些数据目前尚未对执行流产生任何影响（因为在函数入口），并把它称为 内核状态。完成了PoC原型后并与Syzkaller社区进行讨论，经过讨论和一些更细粒度的测试后发现这个方法本身不合适被用于QA工程师的日常工作，直到2020年，终于完成了通用型模糊测试工具的设计和实现，这个项目被正式命名为<a href="https://www.solidot.org/story?sid=65040" target="_blank">Harbian-QA</a>，这也是VaultFuzzer的前身。后来在一个关于<a href="https://groups.google.com/g/syzkaller/c/yFtW39rcWyQ/m/yXgntBtVAAAJ">可控并发测试议题的讨论中</a>，内容涉及一些和状态相关的内容，在讨论中，Vegard Nossum提出了一种方法，即对结构及成员进行hash来收集数据访问情况，并且在不到24小时内发布他为此开发的GCC plugin的PoC原型。这个方法其实和2020年 Harbian-QA发布的Clang/LLVM以instrumentation的实现内容很相似，但只收集访问结构体及其成员名的hash，Vegard Nossum似乎是为了这个触发并发错误开发的，和 Harbian-QA设计目标有所不同。近期的一篇论文"GREBE: Unveiling Exploitation Potential for LinuxKernel Bugs"中，GREBE声称他们开发了一种<a href="https://hardenedvault.net/zh-cn/blog/2022-08-07-state-based-fuzzer-update/" target="_blank">“内核对象驱动”的模糊测试方法</a>，经过<a href="https://hardenedvault.net/zh-cn/blog/2022-08-07-state-based-fuzzer-update/" target="_blank">HardenedVault团队分析后发现其和Harbian-QA以及Vegard的方案的相似度极高</a>，Vault Labs联系了HardenedLinux曾经的全职maintainer确认GREBE论文作者之一Dongliang Mu不仅长期关注Harbian-QA的进展，甚至曾经就Harbian-QA内容寻求HardenedLinux 的帮助，而Dongliang Mu亦活跃于syzkaller社区，可能也读过Vegard的PoC。遗憾的是，GREBE在更换完这些术语和解释后，声称其设计是自行完成的一种新型内核fuzzer，GREBE论文花了大量篇幅来描述其他Fuzzer无法满足其应用场景的原因，整篇论文即没有引用Harbian-QA也没有引用Vegard的PoC，虽然我们不大清楚现代学术界是怎么运作的，但以常识判断这种”copy+paste+replace"并且不给出引用显然是有悖于柏拉图时代的学院派。希望RR坚信的HardenedVault应该保持“We’re neither academia bitch nor industry leech.“并不是红药丸的选择，不是吗？"</i>
</div>
