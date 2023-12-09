[#]: subject: "A Sleek-Looking Linux App to Manage Your Personal Finance"
[#]: via: "https://news.itsfoss.com/denaro/"
[#]: author: "Sourav Rudra https://news.itsfoss.com/author/sourav/"
[#]: collector: "lujun9972/lctt-scripts-1700446145"
[#]: translator: "GlassFoxowo-Dev"
[#]: reviewer: "wxy"
[#]: publisher: "wxy"
[#]: url: "https://linux.cn/article-16449-1.html"

一款外观时尚的用于管理个人财务的 Linux 应用
======

![][0]

> Linux桌面的完美应用，用于轻松管理财务！

个人财务如果管理得当，对于财务状况大有裨益。许多人意识到这一点后，开始采取积极措施来保持财务状况良好。

由于这一点，**我们最近看到了个人财务管理应用的崛起**，这些应用凭借提供的功能已经引起了广泛关注。

但是，**许多现有的应用都是专有的**，这导致人们对于他们的财务数据可能如何处理产生了不确定性，尤其是如果它们同步到云中。

幸运的是，**我们有一些出色的开源选择**。通过这次初步了解，我们将看到其中一款，“**Denaro**”，**一款适用于Linux的个人财务管理应用**。

### Denaro：概览 ⭐

![][1]

用 C# 编写的 Denaro 是**一款整洁的小应用，可轻松管理你的财务**。它是**完全开源**的，依赖社区的贡献来推动其发展。

其中一些**关键功能**包括：

  * 轻松筛选交易
  * 导入/导出功能
  * 多账户支持

#### 初次印象 👨‍💻

我使用 Flathub 商店提供的可用包安装了 Denaro ，它**与我搭载 GNOME 42 的系统集成良好**。

**该应用程序是以 GNOME 为基础设计的**，并针对默认的 Adwaita 主题进行了优化。

第一次启动时，我被问候了“下午好！”并提供了创建新账户或打开现有账户的选项。

> 📋 请注意，账户是存储在本地的，而不是在任何云服务上。

![][2]

我选择创建一个新账户，然后我看到了**快速设置向导**。

![][3]

我输入了账户名称，并将位置设置为“<ruby>文档<rt>Documents</rt></ruby>”，我没有添加密码，但如果你想更好地保护信息，密码也是可选用的。 🧐

![][4]

设置完所有这些后，我可以**选择账户类型**，我可以选择 <ruby>支票<rt>Checking</rt></ruby>、<ruby>储蓄<rt>Savings</rt></ruby> 和 <ruby>商业<rt>Business</rt></ruby>，我选择了储蓄。

我还可以**设置默认交易类型**，并**设置交易提醒阈值**。

![][5]

Denaro 很好地读取了我系统的信息，**自动将货币设置为印度卢比（INR）的 ₹**。

![][6]

然后，我继续填充 Denaro 的一些重要交易，并通过**创建新组**将它们分组，如下所示。

你可以通过单击侧栏中“<ruby>+ 新建<rt>+ New</rt></ruby>”按钮旁边的“<ruby>分组<rt>Groups</rt></ruby>”标题来访问它。你还可以为其**提供描述**和**标记颜色**！

![][7]

完成分组后，我开始**在 Denaro 中输入一些重要的交易**。

我设置了 <ruby>金额<rt>Amount</rt></ruby>，选择了交易类型（<ruby>收入<rt>Income</rt></ruby>/<ruby>支出<rt>Expense</rt></ruby>），设置了 <ruby>日期<rt>Date</rt></ruby> 和 <ruby>重复间隔<rt>Repeat Interval</rt></ruby>，以便它自动记账，因为那是固定费用。

接下来，我将其添加到一个组中，如下所示。燃油费用进入了“旅行”组。

![][8]

该应用还为你提供了**向交易添加注释并上传收据的选项**。如果你问我，这是一个不错的功能。

![][9]

在完成数据输入后，我看到了**一个主屏幕**，其中充满了我输入的所有交易，中间有**有用的可视化图表**（下文更多介绍）。

我可以通过取消选中特定的类别和组来排序信息，甚至可以使用**提供的搜索栏**搜索特定的交易。

如果你想知道；**如何添加新交易？**

你看到下面那个大大的蓝色按钮，上面写着“<ruby>+ 新建<rt>+ New</rt></ruby>”，你可以使用它来创建新交易。

![猫税/分期付款是我从不轻视的费用。 🐱][10]

至于**数据如何可视化**，Denaro 展示了**四种不同的可视化视图**，包括一个图表、一个图形和两个饼图。

![][11]

Denaro 还具有**多账户功能**，你可以创建多个账户，甚至可以使用“<ruby>转账<rt>Transfer</rt></ruby>”功能**在它们之间转移资金**。

通过单击“<ruby>操作<rt>Actions</rt></ruby>”按钮并单击“<ruby>转账<rt>Transfer Money</rt></ruby>”来访问它。

![][12]

引起我的另一个注意的是**Denaro 上的货币换算器**。它**列出了所有主要货币**，并有一个便捷的“切换”按钮来更改换算的目标。

![][13]

**总的来说，这是一个令人印象深刻的个人财务管理应用程序**。

从我的体验来看，**用户体验非常直观**，大多数用户应该能够轻松使用它。

### 📥 下载 Denaro

你可以从 [Flathub 商店][14]、[Snap Store][15] 和 [AUR][16] 获取 Denaro 的最新版本。

> **[Denaro（Flathub）][14]**

关于源代码，你可以访问其 [GitHub 仓库][17]。

💬 你是如何管理个人财务的？你喜欢使用像 Denaro 这样的应用程序吗？请在下方评论中告诉我。

--------------------------------------------------------------------------------

via: https://news.itsfoss.com/denaro/

作者：[Sourav Rudra][a]
选题：[lujun9972][b]
译者：[GlassFoxowo-Dev](https://github.com/GlassFoxowo-Dev)
校对：[wxy](https://github.com/wxy)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://news.itsfoss.com/author/sourav/
[b]: https://github.com/lujun9972
[1]: https://news.itsfoss.com/content/images/2023/11/Denaro.png
[2]: https://news.itsfoss.com/content/images/2023/11/Denaro_1.png
[3]: https://news.itsfoss.com/content/images/2023/11/Denaro_2.png
[4]: https://news.itsfoss.com/content/images/2023/11/Denaro_3.png
[5]: https://news.itsfoss.com/content/images/2023/11/Denaro_4.png
[6]: https://news.itsfoss.com/content/images/2023/11/Denaro_5.png
[7]: https://news.itsfoss.com/content/images/2023/11/Denaro_6.png
[8]: https://news.itsfoss.com/content/images/2023/11/Denaro_7.png
[9]: https://news.itsfoss.com/content/images/2023/11/Denaro_8.png
[10]: https://news.itsfoss.com/content/images/2023/11/Denaro_9.png
[11]: https://news.itsfoss.com/content/images/2023/11/Denaro_10.png
[12]: https://news.itsfoss.com/content/images/2023/11/Denaro_11.png
[13]: https://news.itsfoss.com/content/images/2023/11/Denaro_12.png
[14]: https://flathub.org/apps/org.nickvision.money
[15]: https://snapcraft.io/denaro
[16]: https://aur.archlinux.org/packages/denaro
[17]: https://github.com/nickvisionapps/denaro
[0]: https://img.linux.net.cn/data/attachment/album/202312/07/103124xo86aq504q6mkokg.jpg