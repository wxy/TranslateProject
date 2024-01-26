[#]: subject: "Mastering Nautilus File Search in Linux Desktop"
[#]: via: "https://itsfoss.com/nautilus-file-search/"
[#]: author: "Sreenath https://itsfoss.com/author/sreenath/"
[#]: collector: "lujun9972"
[#]: translator: "geekpi"
[#]: reviewer: "wxy"
[#]: publisher: "wxy"
[#]: url: "https://linux.cn/article-16583-1.html"

掌握 Linux 桌面中的 Nautilus 文件搜索
======

![][0]

> 使用 GNOME 的 Nautilus 文件搜索，通过这些方便的提示改善您的文件搜索体验，成为一名专业的搜索者。

GNOME 的 Nautilus 文件管理器功能丰富。

不信？看看这篇文章，你就会知道如何将 [Nautilus 的全部功能][1] 发挥到极致。

文件搜索是 Nautilus 被忽视的功能之一。没有多少 Linux 用户充分发挥了它的潜力。

因此，我编写了本教程，与大家分享一些使用 Nautilus 文件管理器中文件搜索选项的技巧。

我知道经验丰富的 Linux 用户可以使用终端中的 [find 命令][2] 实现相同的目的，但许多桌面用户更喜欢使用 GUI。

让我们从最简单的搜索选项开始。

### 按名称搜索文件

打开 Nautilus 并单击顶部栏上的放大镜。这将打开一个搜索栏，你可以在其中输入查询字符串。

当你输入时，搜索结果会不断完善，并在输入完整文件名时进行匹配。

![在 Nautilus 中搜索][3]

> 💡 搜索在当前目录及其子目录中执行。可以启用 [隐藏文件视图][4]，将隐藏文件包含在搜索结果中。

### 根据时间搜索文件

使用 Nautilus，你可以根据文件的创建、修改或上次访问的时间过滤搜索。

为此，请单击搜索按钮并开始输入。当你开始输入时，你会注意到搜索按钮附近有一个下拉菜单。点击它。这将为你提供一个菜单，其中包含用于过滤搜索的选项。

![单击下拉菜单][5]

单击下拉菜单上的 “<ruby>选择日期<rt>Select Dates</rt></ruby>” 按钮。另外，选择选项 “<ruby>文件名<rt>File Name</rt></ruby>” 以按文件名匹配。

![按日期搜索的设置][6]

这将为你提供一个扩展菜单，你可以在其中选择文件创建、修改或上次访问的日期。

![设定标准][7]

在这里，如果你想设置自定义日期，请单击日历图标，如下图所示：

![点击日历图标][8]

现在，你将看到一个小日历，并可以相应地选择日期。

![选择日期][9]

从列表中设置你选择的日期后，你可以看到搜索栏上应用的条件，并向你显示基于该条件的文件。

![应用日期标准][10]

### 根据文件类型搜索文件

你还可以根据文件类型过滤搜索。假设你正在寻找 PDF 文件。

与上一步一样，单击搜索图标并开始输入文件名。现在，从下拉菜单中，单击 “<ruby>任何<rt>Anything</rt></ruby>” 选项并选择 “<ruby>文件名<rt>File Name</rt></ruby>”。

![根据文件类型搜索][11]

从展开的视图中选择要搜索的文件类型。在这里，我选择了 “PDF/Postscript”。

![设置所需的文件类型][12]

选择所需的文件类型后，你可以在搜索栏上看到应用的条件。你还将看到相应的结果。

![应用文件类型标准][13]

在搜索选项中没有找到所需的文件类型？向下滚动到底部并单击 “<ruby>其他类型<rt>other types</rt></ruby>”。

![获取更多文件类型][14]

这将为你提供更多文件类型。

![列出更多文件类型][15]

### 搜索文件内容，而不是名称

默认情况下，根据文件名执行文件搜索。如果你想知道是否有包含特定单词的文件，Nautilus 也允许你这样做。

首先，单击搜索图标并开始输入。现在，与前面的部分一样，转到下拉菜单。

在下拉菜单中，不要选择 “<ruby>文件名<rt>File Name</rt></ruby>”，而是选择 “<ruby>全文<rt>Full Text</rt></ruby>”。

现在，你可以搜索特定字符串并根据特定日期或文件类型进行搜索过滤。过滤的方法与前面提到的相同。

![选择“全文”选项][16]

在这里，我使用了字符串 “text to be”，你可以看到列出了几个具有该特定字符串的文件。另外，你可以看到，该部分也突出显示。

### 仅搜索文件或仅搜索文件夹

默认情况下，Nautilus 会搜索文件和文件夹。你可以将搜索细化为文件或文件夹。

为此，请在下拉菜单中选择 “<ruby>文件名<rt>File Name</rt></ruby>”，然后从类型列表中选择 “<ruby>文件<rt>Files</rt></ruby>” 或 “<ruby>文件夹<rt>Folders</rt></ruby>”，如下所示。

![仅在文件或文件夹中搜索][17]

这将根据你的选择过滤结果。

### 应用多个过滤器

你可以将日期过滤器和类型过滤器组合在一起以获得更精确的搜索。为此，请从各自的下拉列表中选择每个条件。

你可以在下面的截图中看到，我已经搜索了包含字符串 “to be search” 的文件。我应用的标准是 1 天内创建的 PDF 文件。

![应用多个过滤器][18]

### 更多 Nautilus 提示和调整

Nautilus 足以满足大多数搜索场景。如果你需要更多，还有专用的 GUI 工具，可让你执行桌面范围的自定义搜索。

> **[ANGRYsearch - 用于 Linux 的快速搜索图形用户界面工具][19A]**

想要更多这样的 Nautilus 技巧吗？ [以 root 身份打开文件][20] 怎么样？

> **[在 Nautilus 文件管理器中以管理员身份打开文件和文件夹][20]**

或者将终端的功能与文件管理器结合起来？

> **[在 Linux 中混合搭配终端与 Nautilus 文件管理器][20A]**

这里还有更多此类提示。请自行查看。

> **[在 Linux 中调整 Nautilus 文件管理器的 13 种方法][20B]**

我希望你喜欢这些技巧，它们有助于更好地改善你的桌面 Linux 体验。

你还知道其他这样酷的技巧吗？ 请在评论中分享。

*（题图：DA/77ae519f-e942-42b0-9808-4af943b168cb）*

--------------------------------------------------------------------------------

via: https://itsfoss.com/nautilus-file-search/

作者：[Sreenath][a]
选题：[lujun9972][b]
译者：[geekpi](https://github.com/geekpi)
校对：[wxy](https://github.com/wxy)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://itsfoss.com/author/sreenath/
[b]: https://github.com/lujun9972
[1]: https://itsfoss.com/nautilus-tips-tweaks/
[2]: https://linuxhandbook.com/find-command-examples/?ref=itsfoss.com
[3]: https://itsfoss.com/content/images/2023/08/Click-on-the-search-button-and-start-typing.png
[4]: https://itsfoss.com/show-hidden-files-linux/
[5]: https://itsfoss.com/content/images/2023/08/Access-more-search-options.png
[6]: https://itsfoss.com/content/images/2023/08/click-on-time-option-to-get-expanded-list.png
[7]: https://itsfoss.com/content/images/2023/08/Search-according-to-date-and-time.png
[8]: https://itsfoss.com/content/images/2023/08/click-on-calendar-icon.png
[9]: https://itsfoss.com/content/images/2023/08/select-date-from-calendar.png
[10]: https://itsfoss.com/content/images/2023/08/Showing-search-criterea-date-on-search-result.png
[11]: https://itsfoss.com/content/images/2023/08/click-on-type-option-to-get-expanded.png
[12]: https://itsfoss.com/content/images/2023/08/Search-based-on-file-type-like-pdf.png
[13]: https://itsfoss.com/content/images/2023/08/showing-search-criteria-type-on-search-result.png
[14]: https://itsfoss.com/content/images/2023/08/click-on-other-type.png
[15]: https://itsfoss.com/content/images/2023/08/complete-list-of-types.png
[16]: https://itsfoss.com/content/images/2023/08/Search-inside-the-file.png
[17]: https://itsfoss.com/content/images/2023/08/search-for-only-folders-or-only-files.png
[18]: https://itsfoss.com/content/images/2023/08/applied-multiple-criteria.png
[19]: https://itsfoss.com/content/images/size/w256h256/2022/12/android-chrome-192x192.png
[19A]: https://itsfoss.com/angrysearch/
[20]: https://itsfoss.com/open-nautilus-as-administrator/
[20A]: https://itsfoss.com/terminal-nautilus-combination/
[20B]: https://itsfoss.com/nautilus-tips-tweaks/
[0]: https://img.linux.net.cn/data/attachment/album/202401/25/155635ocrk3q8dgg3rkkgh.jpg