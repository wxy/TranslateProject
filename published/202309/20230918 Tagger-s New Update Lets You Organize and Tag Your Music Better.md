[#]: subject: "Tagger's New Update Lets You Organize and Tag Your Music Better"
[#]: via: "https://news.itsfoss.com/tagger-2023-9-release/"
[#]: author: "Sourav Rudra https://news.itsfoss.com/author/sourav/"
[#]: collector: "lujun9972/lctt-scripts-1693450080"
[#]: translator: "geekpi"
[#]: reviewer: "wxy"
[#]: publisher: "wxy"
[#]: url: "https://linux.cn/article-16217-1.html"

Tagger 的新更新可让你更好地组织和标记音乐
======

![][0]

> 使用 Tagger 来标记你的音乐？ 现在，它增加了新功能和修复。

Tagger 已发布新版本，其中包含大量有用的改进！

对于那些不知道的人来说，Tagger 是**一款专注于流行音乐文件类型的开源 [标签编辑器应用][1]**，支持 MP3、OGG、FLAC、WAV 等音乐文件。

它可用于**向音乐文件添加重要的元数据**，例如专辑封面、艺术家/发行商信息、发行年份，甚至自定义属性。

让我们看看这个新版本的 Tagger 能提供什么。

### 🆕 Tagger V2023.9.1：有什么新变化？

![][2]

Tagger 采用 C# 语言编写，**它出现自 2021 年底**，并且一直在定期进行改进。

在 **Tagger V2023.9.1** 版本中添加了多项改进。

首先，它包括了**更新的翻译**，要感谢 [Weblate][3] 上的用户。

然后还有**新添加的功能**，可以在 Tagger 中**打开、管理和创建播放列表**。这是为了更容易地同时处理许多音乐文件，从而“<ruby>音乐文件夹<rt>Music Folder</rt></ruby>”现在被称为“<ruby>音乐库<rt>Music Library</rt></ruby>”。

接下来，**同步歌词时间戳现在以 “mm:ss.xx” 格式显示**，遵循 [LRC][4] 规范，并且可以指定 “**hh:mm:ss**” 和 “**mm:ss.xx**” 格式，允许 Tagger 对其进行转换。

此外，Tagger 现在在排序时**在音乐文件列表中显示标题**，为了获得更有条理的文件视图，**主窗口大小在应用重新启动时不会丢失**，并且 **LRC 文件现在可以正确导入**。

有关更多技术细节，你可以参考其 [发行说明][5]。

### 📥 下载Tagger V2023.9.1

你可以通过选择可用的软件包之一来获取最新版本的 Tagger，如下所示：

   * [Snap][6]
   * [Flatpak][7]
   * [AUR 包][8]

对于 Ubuntu，你还可以运行以下命令来安装它：

````
sudo snap install tagger
````

> 💡 当我们谈论添加元数据的应用时，还有 [元数据清理器][9]。它允许你清除最流行的文件类型中的元数据，这与 Tagger 完全相反。

💬 你以前用过 Tagger 吗？ 你对此的体验如何？ 在评论区分享你的观点。

*（题图：MJ/02d910b8-80d1-4802-8125-11ebc45287bf）*

--------------------------------------------------------------------------------

via: https://news.itsfoss.com/tagger-2023-9-release/

作者：[Sourav Rudra][a]
选题：[lujun9972][b]
译者：[geekpi](https://github.com/geekpi)
校对：[wxy](https://github.com/wxy)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://news.itsfoss.com/author/sourav/
[b]: https://github.com/lujun9972
[1]: https://en.wikipedia.org/wiki/Tag_editor
[2]: https://news.itsfoss.com/content/images/2023/09/Tagger.png
[3]: https://weblate.org/en/
[4]: https://en.wikipedia.org/wiki/LRC_(file_format)
[5]: https://github.com/NickvisionApps/Tagger/releases/tag/2023.9.1
[6]: https://snapcraft.io/tagger
[7]: https://flathub.org/apps/org.nickvision.tagger
[8]: https://aur.archlinux.org/packages/tagger
[9]: https://itsfoss.com/metadata-cleaner/
[0]: https://img.linux.net.cn/data/attachment/album/202309/22/224653c080ssjgi8ba808c.jpg