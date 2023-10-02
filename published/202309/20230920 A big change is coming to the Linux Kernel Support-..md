[#]: subject: "A big change is coming to the Linux Kernel Support…."
[#]: via: "https://news.itsfoss.com/linux-kernel-support/"
[#]: author: "Sourav Rudra https://news.itsfoss.com/author/sourav/"
[#]: collector: "lujun9972/lctt-scripts-1693450080"
[#]: translator: "ChatGPT"
[#]: reviewer: "wxy"
[#]: publisher: "wxy"
[#]: url: "https://linux.cn/article-16211-1.html"

Linux 内核支持周期即将发生一项重大变革！
======

![][0]

> 从文字描述上看，它对用户产生的影响将如何呢？你有何看法呢？

<ruby>[欧洲开源峰会][1]<rt>Open Source Summit Europe</rt></ruby> 刚刚开幕，我们开始看到围绕 Linux 和开源软件的一些有趣动态。

其中一项新闻是关于未来将如何处理 Linux 内核的 [长期支持][2]（LTS）版本。

我们来看一下即将进行的更迭。

**新变化：** 在峰会上，Linux 开发者和 [LWN][3] 执行编辑 Jonathan Corbett 宣布，**Linux 内核的 LTS 周期即将从原先的六年缩短至两年**！

目前，有 **六个 LTS 版本的 Linux 内核**，即 4.14、4.19、5.4、5.10、5.15 和 6.1。

在将来，继 4.14 之后，当 LTS 状态的下两个版本被淘汰时，**它们将不会被其他内核版本所取代**。

> 📋 你可以查阅 [Linux 内核归档][4] 来了解目前 LTS 版本 Linux 内核预计的终止支持日期。

长期支持内核：

版本	| 维护者	| 发布于	| 计划终止日期
--:|:--:|:--:|:--
6.1	| Greg Kroah-Hartman & Sasha Levin	| 2022-12-11	| 2026 年 12 月
5.15 | Greg Kroah-Hartman & Sasha Levin |2021-10-31 |	2026 年 10 月
5.10 | Greg Kroah-Hartman & Sasha Levin | 2020-12-13 |	2026 年 12 月
5.4 | Greg Kroah-Hartman & Sasha Levin | 2019-11-24 |	2025 年 12 月
4.19 | Greg Kroah-Hartman & Sasha Levin | 2018-10-22 |	2024 年 12 月
4.14 | Greg Kroah-Hartman & Sasha Levin | 2017-11-12 |	2024 年 1 月

**时机选择：** Jonathan 提到的理由之一是，**并不是很多人使用旧版本的 Linux 内核**，因此这些版本没必要继续进行维护。

我对此表示同意。然而，肯定有些人对此举动感到不满。

但是，这个决策的推进主要是由于 **Linux 代码维护人员过度劳累的大问题**。

你看，对于一个 LTS 版本的代码进行检查和改善是一项重任务，需要消耗大量的时间和精力，而问题就出在这里。

据 Jonathan 所说，维护人员面临的 **两个大挑战** 分别是：大部分 **维护人员并未得到酬劳以维护 Linux 内核**，以及采用 “[Fuzzing][5]” 技术寻找问题，虽然有所帮助，但有时也可能揭示出许多小问题，需要维护人员花费更多的精力。

看到这样的情况，维护人员容易感到疲劳，对吧？🙁

当被问及 **维护人员如何得到帮助？** 时，Jonathan 建议他们与雇主进行沟通，把 Linux 内核维护工作转为付费工作。

他还补充说，

> 如果公司希望继续从 Linux 中获益，就需要意识到他们必须向 Linux 回馈。

总的来说，此次变革将减轻维护人员的负担，但依赖于旧版本 Linux 内核的系统可能会承受不获得关键更新的风险。

这可能会对大部分用户产生影响，或可能不会，但对某些组织来说，可能会带来些许不便。

💬 你怎么看？在下方评论区分享你的想法吧。

*新闻来源：[ZDNET][6]*

*（题图：MJ/47a40c0f-3a3c-4534-98fe-3c986e9a881c）*

--------------------------------------------------------------------------------

via: https://news.itsfoss.com/linux-kernel-support/

作者：[Sourav Rudra][a]
选题：[lujun9972][b]
译者：ChatGPT
校对：[wxy](https://github.com/wxy)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://news.itsfoss.com/author/sourav/
[b]: https://github.com/lujun9972
[1]: https://events.linuxfoundation.org/open-source-summit-europe/
[2]: https://itsfoss.com/long-term-support-lts/
[3]: https://lwn.net/
[4]: https://kernel.org/category/releases.html
[5]: https://en.wikipedia.org/wiki/Fuzzing
[6]: https://www.zdnet.com/article/long-term-support-for-linux-kernel-to-be-cut-as-maintainence-remains-under-strain/
[0]: https://img.linux.net.cn/data/attachment/album/202309/21/085832oy6xi3jqrm44s9xg.jpg