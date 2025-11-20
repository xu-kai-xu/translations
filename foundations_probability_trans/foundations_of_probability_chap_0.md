# 概率理论基础

根据英文第二版翻译。

作者：Andrey Nikolaevich Kolmogorov

英文版本译者：Nathan Morrison

作者小传：A.T. Bharucha-Reid

ISBN：9780486821597 

[TOC]



## 编者注

在准备Kolmogorov（柯尔莫戈洛夫）教授这项基础工作的英文翻译稿的过程中，我们参考了1933年发表在《Ergebnisse Der Mathematik》上的德文原版专题论文**Grundbegriffe der Wahrscheinlichkeitrechnung**（概率论的基本概念），以及1936年出版的俄文译本（由G. M. Bavli翻译）。

编者感谢他两位朋友和他侄女的帮助。

编者感谢 Roy Kuebler 提供的自己由德文翻译的英文版本。

## 前言

本专题论文的目的在于，给概率理论以公理化的基础。作者给自己设定的任务是，将概率论的基本概念（直到最近[^0.1]这些概念还被认为是相当奇怪的概念）置于现代数学的一般概念之中。

如果不先介绍 Lebesgue（勒贝格）关于测度和积分的理论，以上任务几乎是无法完成的。在 Lebesgue 发表他的研究成果之后，集合的度量与事件的概率之间的联系，以及函数的积分与随机变量的数学期望之间的联系，变得显而易见。这些联系为进一步的推广提供了可能，例如，独立随机变量的各种性质被看作与正交函数的相应性质完全类似。但如果要将概率论置于以上的可类比的联系的基础之上，仍然有必要使度量和积分理论独立于勒贝格所突出的几何元素。这项工作由 Fréchet 完成[^2]。

虽然基于上述一般观点的概率论理论在某些数学家中已经存在了一段时间，但缺乏一部完整的、不依赖外部复杂概念的系统性阐述。（参考文献中的 Fréchet 的著作 [^0.2]，给出了一个比较完整的论述。）

我想请大家注意那些超出了专家们早已熟知的以上提到的内容，包括：

1.   有限维空间中的概率分布（第三章，第 4 节）；
2.   对某个参数的数学期望的微分和积分（第四章，第 5 节）；
3.   条件概率和条件期望（第五章）；

这些新问题是随着一些完全具体的物理问题产生的[^0.3]。

第六章包含了对 A. Khinchine 和作者关于普通和强大数定律适用性限制的一些结果的概述，但没有提供证明。参考文献中列举了一些近期的作品。

作者对 Khinchine 的致谢，后者通读全文后给予了一些改进建议。

Kljasma near Moscow

1933年复活节

[^0.1]: 原始德文版本发表于1933年。
[^0.2]: 暂不确定此人是谁。
[^0.3]: 原文脚注1，Zur Statistik der kontinuierlichen Systeme und des zeitlichen Verlaufes der physikalischen Vorgange. Phys. Jour, of the USSR, Vol. 3, 1933, pp. 35-63. 标题英文为 *On the statistics of continuous systems and the temporal evolution of physical processes*.

