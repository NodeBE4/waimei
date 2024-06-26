---
layout: post
title: "VaultHSM：OpenPGP智能卡中确定性 ECDSA的测试方法"
date: 2021-11-03T13:57:38.000Z
author: Solidot
from: https://www.solidot.org/story?sid=69490
tags: [ Solidot ]
categories: [ Solidot ]
---
<!--1635947858000-->
[VaultHSM：OpenPGP智能卡中确定性 ECDSA的测试方法](https://www.solidot.org/story?sid=69490)
------

<div>
<a href="http://https://hardenedvault.net/">HardenedVault</a> 写道<i> "DSA 型签名算法（包括 ECDSA）的原始实现中需要一个和私钥属于同种数学对象（GF(p) 的元素，p 为素数）的随机数，该随机数必须同时满足以下三个性质：1）随机性：无法仅通过被签名数据（以下称“载荷”）和生成的签名推算出来。2）机密性：不可泄露到签名过程之外。3）唯一性：该随机数对不同的载荷必须不同。否则，攻击者将有可能通过载荷与签名推算出私钥。如果该随机数来自一个有缺陷的随机数发生器，则随机性和唯一性会变得难以保证——攻击者可能通过收集足够多的载荷——签名对找到随机数发生器的规律，进而推算出私钥，虽然行业用户认为这是“可忍受”的缺陷直到<a href="https://link.zhihu.com/?target=https%3A//eprint.iacr.org/2020/615" class=" wrap external" target="_blank" rel="nofollow noreferrer" data-za-detail-view-id="1043" style="text-decoration-line: none; cursor: pointer; border-bottom: 1px solid rgb(128, 128, 128);">LadderLeak</a>漏洞的公开披露彻底让真相浮出水面，在最坏的情况下，攻击者只需要付出30万美金就可以破解P-224的密钥。由于开源的安全ECDSA实现进展并不顺利，Vault Labs给出了<a href="https://zhuanlan.zhihu.com/p/429119101" target="_blank">测试缺陷的方法和临时安全解决方案</a>： 确保所有你使用的证书是&gt;= P-256或者RSA（有其他风险需要考量）以及安全人员不要漏掉对没有接入互联网的服务的审计。"</i>
</div>
