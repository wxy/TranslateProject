[#]: subject: "What is Super Key in Linux?"
[#]: via: "https://itsfoss.com/super-key/"
[#]: author: "Sagar Sharma https://itsfoss.com/author/sagar/"
[#]: collector: "lujun9972/lctt-scripts-1700446145"
[#]: translator: "ChatGPT"
[#]: reviewer: "wxy"
[#]: publisher: "wxy"
[#]: url: "https://linux.cn/article-16404-1.html"

Linux 黑话解释：Linux 中的 Super 键是什么？
======

![][0]

> 在本次 Linux 黑话解释系列的这一篇，我们会一起来探索 Linux 中的 `Super` 键（或称其为 `Meta` 键）。

当你在网上浏览 Linux 教程时，你可能会遇到 “`Super` 键” 这个术语，对于 Linux 的初学者来说，这可能会引起混淆。

概括地说，如果你的电脑预装了 Windows，那么带有 Windows 标志的 `Windows` 键就是 `Super` 键。

如果你使用的是苹果电脑，那么带有 `⌘` 符号的 `command` 键就是你的 `Super` 键。

![下面这个就是你的 Super 键（或者 Meta 键）][1]

很简单吧？

但是，为什么要将其命名为 `Super` 键呢？毫无疑问，背后一定有一些有趣的故事。

那么，让我们一起按下 `Super` 键，发掘更深层次的故事吧。

### Super 键背后的想法

它首次出现在 “space-cadet” 键盘中，这款键盘是在 1978 年为 [Lisp 机器][2] 设计的，其主要目的是用来模拟 `Meta` 键。（LCTT 译注：这款键盘的独特之处在于它设有七个修饰键，包括 `Shift`、`Control`、`Meta`、`Super`、`Hyper`，用户可以通过组合这些修饰键与其他键来输入更多的字符和命令，它对现代计算机键盘的发展产生了重要影响。）

`Meta` 键在 Emacs 编辑器中是非常重要的一个部分，但在当时的现代键盘中却未能配备实体的 `Meta` 键，因而人们常常通过不同的按键绑定来模仿其功能。

`Super` 键的引入，解决了这个问题，由此我们有了一个真实的 `Super` 键。

快进到 1994 年，当时 `Windows` 键首次在 [微软自然键盘][3] 上出现，它被用来迅速打开“开始”菜单。从 1996 年开始，将 `Meta` 键映射到 `Windows` 键成为了普遍的做法。

### Super 键的一般使用情况

当你在 Ubuntu 桌面上按下 `Super` 键时，它会显示活动概览，让你全面了解每个窗口正在进行的活动：

![在 Ubuntu 中按下 Super 键获得活动概览][4]

但你要知道，除了预览正在进行的活动，你其实还可以做更多。

比如，你可以同时按下 `Super` 键和 `Tab` 键，调出应用切换器，从而在正在运行的应用之间切换。

![][5]

下面列举了一些可以利用 `Super` 键的快捷键（在 Ubuntu 23.10 内部测试通过）：

> 📋 如果你在使用的是基于 Ubuntu 的发行版，其中的某些快捷键可能并不会按照预期那样工作，因为发行版维护者可能已经将该快捷键指定为另一个任务。

快捷键 | 描述
---|---
`Super` | 打开活动概览
`Super` + `Tab` | 切换开放应用
`Super` + `D` | 显示桌面（最小化所有窗口）
`Super` + `A` | 打开应用菜单
`Super` + `S` | 显示快速设定
`Super` + `←` | 将活动窗口移至屏幕的左半部分
`Super` + `→` | 将活动窗口移至屏幕的右半部分
`Super` + `↑` | 最大化活动窗口
`Super` + `↓` | 最小化活动窗口
`Super` + `L` | 锁定屏幕

这些操作实在太方便了，对吧？

### 通过快捷键提高生产效率

对于新接触 Ubuntu 的你，下列的一些有帮助的快捷键值得一试：

> **[Ubuntu 用户应该知道的 13 个快捷键][6]**

如果你刚开始使用终端，我会推荐你学习 [Linux 终端的基本快捷键][7]：

> **[专业用户喜欢使用的 21 个 Linux 终端快捷键][7]**

我希望这篇文章能给你带来宝贵的信息，使你对 Super 键有更深入的了解 ;)

*（题图：MJ/9b9a1146-0e76-459a-880d-b1a1a4fa5f1e）*

--------------------------------------------------------------------------------

via: https://itsfoss.com/super-key/

作者：[Sagar Sharma][a]
选题：[lujun9972][b]
译者：[ChatGPT](https://linux.cn/lctt/ChatGPT)
校对：[wxy](https://github.com/wxy)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://itsfoss.com/author/sagar/
[b]: https://github.com/lujun9972
[1]: https://itsfoss.com/content/images/2023/11/keyboard-linux.jpg
[2]: https://en.wikipedia.org/wiki/Lisp_machine
[3]: https://en.wikipedia.org/wiki/Microsoft_ergonomic_keyboards#Natural_Keyboard
[4]: https://itsfoss.com/content/images/2023/11/Get-activities-overview-in-Ubuntu-by-pressing-the-super-key.png
[5]: https://itsfoss.com/content/images/2023/02/App-Switch.png
[6]: https://itsfoss.com/ubuntu-shortcuts/
[7]: https://itsfoss.com/linux-terminal-shortcuts/
[0]: https://img.linux.net.cn/data/attachment/album/202311/21/211946e9resh69paphei8i.png