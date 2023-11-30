[#]: subject: "rlxOS: An Indepdent Immutable Linux Distro With Xfce Desktop"
[#]: via: "https://news.itsfoss.com/rlxos/"
[#]: author: "Sourav Rudra https://news.itsfoss.com/author/sourav/"
[#]: collector: "lujun9972/lctt-scripts-1700446145"
[#]: translator: "ChatGPT"
[#]: reviewer: "wxy"
[#]: publisher: "wxy"
[#]: url: "https://linux.cn/article-16415-1.html"

rlxOS：一个独立的不可变 Linux 发行版，具有 Xfce 桌面
======

![][0]

> 这是一款具有良好的外观和感觉，独立的不可变发行版。

[不可变 Linux 发行版][1] 的市场在稳步增长。

只在今年，我们就见证了像 [Fedora Onyx][2]、[blendOS v3][3] 这样的新成员，以及 Ubuntu 24.04 LTS 将会出现的 [基于 Snap 的不可变 Ubuntu 桌面][4]。

在这篇 [初次体验][5] 的文章里，我们将探索 [rlxOS][6]，它是一款自行建制的不可变发行版。

现在，让我们深入了解一下。

> 🚧 这个发行版相当新，可能无法作为日用主系统的替换产品。

### rlxOS：概述 ⭐

![][7]

rlxOS 以**从零开始构建**为自豪，作为一个 [独立的 Linux 发行版][8]，能更好地控制核心和工作部分。作为不可变的发行版，它实现了一种 [滚动发布][9] 的方式，从而用户在面对大的更新时无需重新安装。

其**主要特点**包括：

  * **不可变性**
  * **利用** [Ostree][10]
  * **关注隐私**
  * **原生支持 Flatpak**

如果你还不知道，不可变发行版可以让你在不影响系统核心的情况下进行变更。你可以将其视为分层变更，因此一个变更并不会影响另一个。

为了使这个实现，rlxOS 使用了一个软件更新守护程序（[swupd][11]），这个程序保留了操作系统的两个版本（在更改前后），你可以按照 [文档][11] 进行一些在重启后会消失的更改。

这个守护程序也会让你有不同层的软件包。根据官方网站，该功能在稳定版本中还未推出。

另外，你可以轻松地按照 [文档][13] 设置 [Distrobox][12] 容器。

#### 初次印象 👨‍💻

我在使用 [Ubuntu 上的 VirtualBox][15] 的虚拟机（VM）上启动了 rlxOS。安装程序看起来非常舒服，它那种圆角矩形的感觉让我**想起了 GNOME 中** [**Adwaita**][16] **的主题风格**。

![][17]

我在进行过程中**需要手动使用** [GParted][18] **对驱动器进行分区**。首先，我在虚拟驱动器上建立了推荐的 msdos 分区表。

之后，我分了两个不同大小的分区，一个是 ext4 文件系统的 39.5 GB 分区，另一个是 fat32 文件系统的 512 MB 分区。

在这之后，我需要确定 fat32 分区有 `boot` 和 `esp` 标记，这样才能正确的安装 rlxOS。

> 📋 通过右键点击分区并选择“<ruby>管理标志<rt>Manage Flags</rt></ruby>”来设定标记。

![][19]

**安装程序还给出了关于分区的有效提示**，将较大的一个标记为 `Linux`，将较小的一个标记为 `EFI`。

如果你打算在 Windows 系统旁边安装它，你需要小心分区的设定，因为我们还没有在这里进行过测试。

![][20]

然后，确认屏幕会显示出来，揭示**一些重要的最后阶段信息**。我点击 “<ruby>应用<rt>Apply</rt></ruby>” 继续进行。

![][21]

然后，它**需要花费一些时间才能完成安装**。但是，出于一些原因，我在安装过程中能够点击 “<ruby>下一步<rt>Next</rt></ruby>” 和 “<ruby>上一步<rt>Back</rt></ruby>” 选项（我认为这些选项应是灰化的）。

![][22]

我建议你让安装自然进行，不要调整其他任何事情，并等待如下所示的 “<ruby>成功<rt>Success</rt></ruby>” 提示。

![][23]

在重启后，**快速设置向导**开始运行，我输入了用户信息和密码，然后再次重启。

![][24]

在重启后看到了**十分整洁的登录界面**，含有一张漂亮的壁纸，和标题栏常见的一些选项/信息。

![][25]

登录之后，我看到了**一个非常熟悉的桌面界面**，这个界面有**一个类似 Windows 的应用启动器**，和**一栏包含了有用的部件的任务栏**，如语言、通知、网络、节能模式等等。

![][26]

然而，我立刻注意到**rlxOS 预装的应用程序非常的少**。这可以看作一件好事，这取决于你问的人。

但是，我必须说，Xfce 的体验看起来很好。

在我看来，他们可以至少添加任何一款 [开源的微软办公套件替代品][27]，诸如 [LibreOffice][28] 或 [ONLYOFFICE][29]，这样这个发行版会有一个更为完整的体验。但是，当然，这是一个新的发行版，无可挑剔。

查看设置应用，它似乎很好的与系统主题相匹配。

![][30]

rlxOS使用 Xfce 作为其桌面，这是流行的且最小化的桌面环境之一。我测试的稳定版是运行定制化 [Xfce 4.18][31]。

![][32]

如果你过去使用过 Xfce，你会发现 rlxOS 上的版本既熟悉又有些许不同。我用了一段时间，对其所提供的内容很满意，比如多任务处理非常轻松，因为**rlxOS 支持工作空间**。

我只需要通过在任务栏中滚动/点击可以轻松地在工作区之间切换。

尽管这个发行版在这里那里有些小问题，但是它值得一试。在实物机器上的你的**体验会比在 VM 上更好**。

如果你对源代码感兴趣，或者你想要为其做出贡献，你可以查阅其 [GitHub 仓库][33]。

### 📥 下载 rlxOS

在我写这篇文章时，[官方网站][34] 上有**两个版本的 rlxOS 可供下载**。一个是**每月更新的稳定版本**，另一个是**被认为是不稳定的实验版本**。

> **[rlxOS][34]**

💬 你对 rlxOS 有什么看法，你会向他人推荐这款发行版吗？

*（题图：MJ/b045e868-db65-4904-a0e4-0252051296e5）*

--------------------------------------------------------------------------------

via: https://news.itsfoss.com/rlxos/

作者：[Sourav Rudra][a]
选题：[lujun9972][b]
译者：[ChatGPT](https://linux.cn/lctt/ChatGPT)
校对：[wxy](https://github.com/wxy)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://news.itsfoss.com/author/sourav/
[b]: https://github.com/lujun9972
[1]: https://itsfoss.com/immutable-linux-distros/
[2]: https://news.itsfoss.com/fedora-onyx-official/
[3]: https://news.itsfoss.com/blendos-v3-released/
[4]: https://news.itsfoss.com/ubuntu-all-snap-desktop/
[5]: https://news.itsfoss.com/tag/first-look/
[6]: https://rlxos.dev/
[7]: https://news.itsfoss.com/content/images/2023/11/rlxos_1.jpg
[8]: https://itsfoss.com/independent-linux-distros/
[9]: https://itsfoss.com/rolling-release/
[10]: https://en.wikipedia.org/wiki/OSTree
[11]: https://docs.rlxos.dev/system-management/swupd/
[12]: https://itsfoss.com/distrobox/
[13]: https://docs.rlxos.dev/system-management/distrobox/
[14]: https://itsfoss.com/content/images/size/w256h256/2022/12/android-chrome-192x192.png
[15]: https://itsfoss.com/install-virtualbox-ubuntu/
[16]: https://en.wikipedia.org/wiki/Adwaita_(design_language)
[17]: https://news.itsfoss.com/content/images/2023/11/rlxos_2.jpg
[18]: https://gparted.org/
[19]: https://news.itsfoss.com/content/images/2023/11/rlxos_3.jpg
[20]: https://news.itsfoss.com/content/images/2023/11/rlxos_4.jpg
[21]: https://news.itsfoss.com/content/images/2023/11/rlxos_5.jpg
[22]: https://news.itsfoss.com/content/images/2023/11/rlxos_6.jpg
[23]: https://news.itsfoss.com/content/images/2023/11/rlxos_7-1.jpg
[24]: https://news.itsfoss.com/content/images/2023/11/rlxos_8.jpg
[25]: https://news.itsfoss.com/content/images/2023/11/rlxos_10.jpg
[26]: https://news.itsfoss.com/content/images/2023/11/rlxos_11.jpg
[27]: https://itsfoss.com/best-free-open-source-alternatives-microsoft-office/#2-onlyoffice
[28]: https://www.libreoffice.org/
[29]: https://www.onlyoffice.com/
[30]: https://news.itsfoss.com/content/images/2023/11/rlxos_11b.jpg
[31]: https://news.itsfoss.com/xfce-4-18-release/
[32]: https://news.itsfoss.com/content/images/2023/11/rlxos_13.jpg
[33]: https://github.com/itsManjeet/rlxos
[34]: https://rlxos.dev/downloads/
[0]: https://img.linux.net.cn/data/attachment/album/202311/26/175005asnmncwmiscmuems.png