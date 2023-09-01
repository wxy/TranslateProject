[#]: subject: "Easily Take Full Webpage Screenshots in Firefox and Chrome"
[#]: via: "https://itsfoss.com/firefox-screenshot/"
[#]: author: "Sagar Sharma https://itsfoss.com/author/sagar/"
[#]: collector: "lujun9972"
[#]: translator: "geekpi"
[#]: reviewer: "wxy"
[#]: publisher: "wxy"
[#]: url: "https://linux.cn/article-16141-1.html"

在 Firefox 和 Chrome 中轻松截取完整网页截图
======

![][0]

> Firefox 浏览器内置了截屏工具，你可以用它对整个网页进行截屏。Chrome 浏览器也有同样的功能。

截屏来捕获信息是很常见的。

但你知道你可以在 Firefox 中截取整个网页的截图吗？Firefox 附带一个内置的截图工具，允许你截取选定区域、可见屏幕区域甚至整个网页的截图。

这意味着如果你想保存网页供以后参考，你可以快速捕获整个网页。

Chrome 也有截图功能，但稍微复杂一些。

在本教程中，我将引导你完成以下内容：

  * 如何在 Firefox 中截图
  * 如何在 Chrome 中截图
  * 使用 Nimbus 扩展获得比内置的截屏更多的功能

那么让我们从第一个开始。

### 在 Firefox 中截取网页截图

Firefox 的内置工具可让你通过单击选择整个屏幕、整个页面，甚至特定段落。

#### 步骤 1：访问截图工具

要启动截图程序，请在使用 Firefox 时按 `Ctrl + Shift + s`。

如果你不总是能记住快捷方式，也可以从右键单击菜单访问该工具。

![Screenshot tool can also be accessed from right-click context menu][1]

如果你经常截图，那么将该程序添加到工具栏将是一个好主意。为此，你只需执行三个简单步骤：

  1. 首先，右键单击工具栏并选择 “<ruby>自定义工具栏<rt>Customize Toolbar</rt></ruby>” 选项
  2. 找到 “<ruby>截图<rt>Screenshot</rt></ruby>” 程序并将其拖至工具栏
  3. 点击 “<ruby>完成<rt>Done</rt></ruby>” 按钮即可

还困惑吗？ 操作方法如下：

![][2]

启用后，你可以单击刚刚拖动到工具栏的截图图标。

#### 步骤 2：在 Firefox 中截图

当你启动截图工具时，它会提示两个选项：“<ruby>保存整页<rt>Save full page</rt></ruby>” 和 “<ruby>保存可见<rt>Save visible</rt></ruby>”。这里：

  * 保存整页将捕获整个网页
  * 保存可见只会捕获当前帧中可见的内容

但如果你想捕获特定部分，你可以使用鼠标光标选择该部分并保存：

![][3]

如你所见，有两个选项：<ruby>下载<rt>Download</rt></ruby> 或 <ruby>复制<rt>Copy</rt></ruby>（到剪贴板，以便你可以将其粘贴到文档或编辑工具中）。你可以根据你的场景使用其中之一。

### 在 Chrome 中截取网页截图

在 Chrome 中截取全部网页截图比在 Firefox 中要复杂一些，因为它隐藏在开发人员选项下。

不用担心！你将通过以下步骤做到：

  * 打开菜单，进入 “<ruby>更多工具<rt>More Tools</rt></ruby>-><ruby>开发者工具<rt>Developer tools</rt></ruby>”。或者，你可以按 `Ctrl + Shift + l` 进入开发者工具目录。
  * 按 `Ctrl + Shift + p` 并输入 `screenshot`（LCTT 译注：在中文环境中请输入 “屏幕截图”）
  * 选择区域或整个页面，然后回下载截图。

让我向你展示如何做到这一点：

![][4]

这几乎就是 Chrome 所能提供的一切。

### 如何使用扩展程序截图

> ✋ 非自由和开源软件警告！这里讨论的 Nimbus 扩展不是开源的。

如果你想要更多功能，例如添加延迟、水印或符号，那么你必须使用扩展程序。

为此，我建议使用 Nimbus，它几乎可以让你执行任何本地安装的截图工具可以执行的所有操作。

下载 Firefox 版 Nimbus：

> **[Firefox 版 Nimbus][5]**

下载 Chrome 版 Nimbus：

> **[Chrome 版 Nimbus][6]**

> 📋 只有 Nimbus 的 Chrome 扩展具有视频录制功能。

完成安装后，**请务必注册 Nimbus 以启用所有功能。**

单击 Nimbus 扩展图标，你会看到多个选项：

![][7]

你可以选择任何显示的功能，完成后，根据捕获后进行的操作（我选择编辑），它将直接下载截图，打开编辑器或将其发送到任何选定的云提供商。

如果你也将 “<ruby>编辑<rt>Edit</rt></ruby>” 作为捕获后的操作，那么它将打开一个编辑器，你可以在其中对捕获的截图进行编辑：

![][8]

如果你想添加水印、了解/更改快捷方式、更改截图的格式等，请打开 Nimbus 并点击小齿轮按钮：

![][9]

只是一个扩展却有非常酷的功能。不是吗？

> 💡 如果你经常截屏，你可能需要将 Nimbus 扩展固定到任务栏。

### 想要更多功能吗？使用截图工具

如果你不想受到扩展功能的束缚，那么需要尝试具有更多功能的截图工具，这些工具可以在整个系统的任何地方使用。

如果你是 Linux 用户，那么我们有一份关于 [Linux 中截取和编辑截图的最佳工具][10] 的专门指南：

> **[Linux 中截取和编辑截图的最佳工具][10]**

我希望你喜欢这个快速技巧。

（题图：MJ/76cc0d02-fb37-4bd0-94ec-fc249c1f537e）

--------------------------------------------------------------------------------

via: https://itsfoss.com/firefox-screenshot/

作者：[Sagar Sharma][a]
选题：[lujun9972][b]
译者：[geekpi](https://github.com/geekpi)
校对：[wxy](https://github.com/wxy)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://itsfoss.com/author/sagar/
[b]: https://github.com/lujun9972
[1]: https://itsfoss.com/content/images/2023/08/take-screenshot-firefox.png
[2]: https://itsfoss.com/content/images/2023/08/Add-screenshot-feature-to-Firefox-browser-1.gif
[3]: https://itsfoss.com/content/images/2023/08/Capture-specific-part-of-webpage-to-screenshot-in-Firefox.gif
[4]: https://itsfoss.com/content/images/2023/08/Take-screenshots-in-Google-chrome-without-any-extension-2-.gif
[5]: https://addons.mozilla.org/en-US/firefox/addon/nimbus-screenshot/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search
[6]: https://chrome.google.com/webstore/detail/nimbus-screenshot-screen/bpconcjcammlapcogcnnelfmaeghhagj
[7]: https://itsfoss.com/content/images/2023/08/Use-nimbus-extension-to-take-full-screen-screenshots-in-chrome-and-firefox.png
[8]: https://itsfoss.com/content/images/2023/08/Edit-screenshots-captured-in-Firefox-and-Chrome.png
[9]: https://itsfoss.com/content/images/2023/08/Additional-settings-of-Nimbus.png
[10]: https://itsfoss.com/take-screenshot-linux/
[11]: https://itsfoss.com/content/images/size/w256h256/2022/12/android-chrome-192x192.png
[0]: https://img.linux.net.cn/data/attachment/album/202308/30/132752rfrq7af9sqraz76r.jpg