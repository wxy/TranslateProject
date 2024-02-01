[#]: subject: "Linux Kernel 6.7 Release is Loaded With Fixes and a New Filesystem"
[#]: via: "https://news.itsfoss.com/linux-kernel-6-7-release/"
[#]: author: "Sourav Rudra https://news.itsfoss.com/author/sourav/"
[#]: collector: "lujun9972/lctt-scripts-1700446145"
[#]: translator: "ChatGPT"
[#]: reviewer: "wxy"
[#]: publisher: "wxy"
[#]: url: "https://linux.cn/article-16547-1.html"

Linux 内核 6.7 发布，包含众多修复和新的文件系统
======

![][0]

> 这是历来重大的 Linux 内核发布之一，集大量修复和新增功能于一身。

新年伊始，全新 Linux 内核发布！ 🎉

我们在 2024 年以 **Linux 内核 6.7 版本** 的推出开启了新的篇章，这一版本具备许多显著改进，其中包括上一版本遗漏的部分内容。

Linus Torvalds 在 [公告][1] 中解释了假期引发的小幅延误：

> 实际上，我们上周的工作量稍比假期前一周多些，但这不会让我觉得我们需要再进一步推迟发布。
>
> 最后的结果：6.7 版本基于提交数量（超过 17k 的非合并提交，以及 1k+ 的合并提交）来看，已经是我们有史以来发布的最大规模的内核版本之一。然而，额外的第 8 个 rc 版本主要是由于圣诞节假期的时间安排，并非大规模发布所引发的。

### 🆕  Linux 内核 6.7：新的变化

由于 6.7 是**非长期支持版本**，你没有必须要升级到 Linux 内核 6.7 的压力，除非你急于体验 Linux 的尖端技术。

有鉴于此，我们来看看这个版本**关键的亮点**包括了哪些内容：

  * **英特尔的优化**
  * **增强的 RISC-V 支持**
  * **针对 AMD 的特别增强**
  * **众多存储功能的优化**

#### 英特尔的优化

![][3]

首先要讲的是英特尔的 [Meteor Lake][4] 处理器。**Linux 内核 6.7 对于英特尔 Meteor Lake 图形提供了原生支持**。在此之前，此项支持还处在 _实验性_ 阶段。但现在，你可以在装备有第一代 [Core Ultra][5] 处理器的笔记本上全面享受到它的优势了。

另外，英特尔即将发布的 [Arrow Lake][6] 和 Lunar Lake 芯片在 [Turbostat][7]（一个用于监测处理器频率、空闲统计等信息的命令行工具）中也做好了规划。

不过，也有一些支持功能被删除。

在 Linux 内核 6.7 中，**不再支持英特尔安腾 IA-64 架构**。这已经计划了好一段时间，现在，终于实现了。

#### 增强的 RISC-V 支持

![][8]

RISC-V 的一大亮点是 **引入了软件阴影调用堆栈**，这旨在保护 CPU 架构免受意外和恶意操作的影响。

此外，**在用户空间对 cbo.zero，以及在基于 ACPI 系统中对** CBO 的支持，还有许多其他杂项修复也同样进行了。这个 [合并请求][9] 中有更多信息。

你还可以阅读关于 <ruby>[阴影堆栈][10]<rt>Shadow Stack</rt></ruby> 的文章，以了解它更多的应用。

#### 针对 AMD 的特别增强

AMD 的 **无缝启动功能已经扩展到支持 Display Core Next 3.0 及以后版本的 GPU**。包括 Radeon RDNA2/RDNA3，以及未来发布的任何 GPU。

此功能使得系统 **平滑过渡，避免了通常随着电源按钮压下后会出现的屏幕闪烁现象**。之前，这个功能仅对 AMD 的 Van Gogh 系列 APU 开放。

接下来是 **错误检测和纠正**（[EDAC][11]）在 [Versal][12] SoC 系列中的引入，它添加了一个 EDAC 驱动，支持在集成的 Xilinx DDR 内存控制器上进行 RAS 功能。

在这个 [提交信息][13] 中，你能了解到关于它如何实施的更多信息，我们在此对 [Phoronix][14] 的发现表示感谢。

#### 众多存储功能的升级

![][16]

我们终于在 Linux 内核 6.7 中迎来了 [Bcachefs][17] 文件系统的引入。如果你对它不熟悉，简单来说，它是一种**写时复制（COW）文件系统**，其重点放在可靠性和稳健表现上。

此外，Btrfs 引入了 **新的三项特性**，F2FS 现在 **支持更大的页面尺寸**，甚至 **IBM 的日志文件系统（JFS）也有所增强**。

#### 🛠️  其它变化及优化

最后，还有其他一些值得注意的变化包括：

  * 停止对 [MIPS AR7][18] 平台的支持。
  * **x86 CPU 微码加载过程** 的改进。
  * 在 [EROFS][19] 上，**MicroLZMA 压缩** 现在被认为是稳定的。
  * 更好地支持 **采用 RISC-V 的** [Milk-V Pioneer][20] 板。
  * 引入 **Nouveau GPU 系统处理器（GSP）**，它为英伟达的 “Turing” 及更新的 GPU 开启了更好的体验途径。

你可以通过阅读 [短日志][1] 或等待在 [内核档案][21] 上发布的更新日志，以了解更多的技术更新。

### 安装 Linux 内核 6.7

如果你在使用如 Arch 或 Fedora 这样的滚动版本发行版，可以期待在发行版开发者的一番测试后，就能收到升级。

对于其他用户，你可以安静等待，或者按照我们的简明教程， **在 Ubuntu 上升级到最新的主线 Linux 内核**：

> 🚧 我们并不建议你手动升级 Linux 内核，除非你的确有某些问题需要解决。

你可以从 [官方网站][21] 获取最新 Linux 内核版本的 tarball。但是请记住，新版本发布后需要一些时间才能下载得到。

> **[Linux 内核 6.7][21]**

💬 你打算升级到 Linux 内核 6.7 吗？你对这个版本有何评价？

*（题图：DA/0e329f2b-a118-4a00-9d90-da036172c271）*

--------------------------------------------------------------------------------

via: https://news.itsfoss.com/linux-kernel-6-7-release/

作者：[Sourav Rudra][a]
选题：[lujun9972][b]
译者：[ChatGPT](https://linux.cn/lctt/ChatGPT)
校对：[wxy](https://github.com/wxy)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://news.itsfoss.com/author/sourav/
[b]: https://github.com/lujun9972
[1]: https://lore.kernel.org/lkml/CAHk-=widprp4XoHUcsDe7e16YZjLYJWra-dK0hE1MnfPMf6C3Q@mail.gmail.com/T/#u
[2]: https://news.itsfoss.com/content/images/size/w256h256/2022/08/android-chrome-192x192.png
[3]: https://news.itsfoss.com/content/images/2024/01/linux-kernel-6-7-chip.png
[4]: https://en.wikipedia.org/wiki/Meteor_Lake
[5]: https://www.intel.com/content/www/us/en/products/details/processors/core-ultra.html
[6]: https://en.wikipedia.org/wiki/Arrow_Lake
[7]: https://www.linux.org/docs/man8/turbostat.html
[8]: https://news.itsfoss.com/content/images/2024/01/linux-kernel-6-7-riscv.png
[9]: https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/commit/?id=d46392bbf5c6ce594669f00b8177f0b34e983f90
[10]: https://en.wikipedia.org/wiki/Shadow_stack
[11]: https://en.wikipedia.org/wiki/Error_detection_and_correction
[12]: https://www.xilinx.com/products/silicon-devices/acap/versal.html
[13]: https://git.kernel.org/pub/scm/linux/kernel/git/ras/ras.git/commit/?h=edac-drivers&id=0fd934580ea3ea91052b999ff75017c3f08b9783
[14]: https://www.phoronix.com/news/AMD-Xilinx-Versal-EDAC-Linux-67
[15]: https://news.itsfoss.com/content/images/2023/04/Follow-us-on-Google-News.png
[16]: https://news.itsfoss.com/content/images/2024/01/linux-kernel-6-7-storage.png
[17]: https://bcachefs.org/
[18]: https://en.wikipedia.org/wiki/Texas_Instruments_AR7
[19]: https://en.wikipedia.org/wiki/EROFS
[20]: https://milkv.io/pioneer
[21]: https://www.kernel.org/
[22]: https://itsfoss.com/content/images/size/w256h256/2022/12/android-chrome-192x192.png
[0]: https://img.linux.net.cn/data/attachment/album/202401/10/160848zkf7awqrclul7m7f.jpg