[#]: subject: "EndeavourOS Galileo: Xfce Out, KDE In"
[#]: via: "https://news.itsfoss.com/endeavouros-galileo/"
[#]: author: "Sourav Rudra https://news.itsfoss.com/author/sourav/"
[#]: collector: "lujun9972/lctt-scripts-1700446145"
[#]: translator: "GlassFoxowo-Dev"
[#]: reviewer: " "
[#]: publisher: " "
[#]: url: " "

EndeavourOS Galileo: 离开 Xfce，拥抱 KDE
======
基于 Arch Linux 的发行版 EndeavourOS 在其最新版本中进行了一些有趣的变更。
一个 [基于 Arch Linux 的最佳用户友好型发行版][1]，EndeavourOS 现已发布版本更新。

代号为 "**Galileo**"，这遵循了我们在过去版本中见过的类似命名方案，比如 [EndeavourOS 'Cassini'][2]。

让我们来看看 "Galileo" 有什么新特性。

## 🆕 EndeavourOS Galileo: 有些什么新东西?

![][3]

尽管这个版本花费了一些时间才发布，但这是**一次重大升级，带来了一些重要的变化**。其中最明显的变化是转向了 KDE Plasma，以及放弃了 Xfce，稍后我们将详细讨论这一点。

**开发者决定使 EndeavourOS 比以前更为轻巧**，削减了一些预设设置，但仍然让你可以轻松地入门并使用 Arch Linux。

这个版本的一些**主要亮点**包括：

  * **欢迎应用改进**
  * **Calamares 安装程序调整**
  * **KDE Plasma 取代 Xfce**



### 欢迎应用改进

![][4]

在安装过程中显示的欢迎应用已经改进，现在它在左下角具有专门的**语言选择选项**。

图标也已更新，安装程序现在默认使用 KDE Plasma。

### Calamares 安装程序调整

![][5]

随着 KDE Plasma 成为默认选择，EndeavourOS Galileo 上的 [Calamares][6] 安装程序**在安装过程中只允许安装一个桌面环境/窗口管理器**。

这是为了减轻安装后出现的冲突软件包问题。**安装完成后，你仍然可以安装其他桌面环境/窗口管理器**。

这还不是全部，**开发者还从安装程序中移除了社区版本**。因此，像 **Sway**、**Qtile**、**BSPWM**、**Openbox** 和 **Worm** 这样的变体无法通过 Calamares 安装了。

它们必须被删除，因为大多数原始开发者已经离开了这个项目，也没有其他人接手。幸运的是，**你仍然可以从它们的 [GitHub 页面][7] 手动安装这些社区版本**。

### KDE Plasma 取代 Xfce

![][8]

未来，**KDE Plasma 将成为默认的桌面环境**，用于运行实时环境和 ISO 上的离线安装选项，取代了 Xfce。

不用担心，**在安装 EndeavourOS 的过程中仍然可以选择安装 Xfce**，前面显示的截图就是证明。

正如开发者所述，这一举措背后的原因是：

> 为了使团队更容易进行开发和维护，我们转而使用 KDE Plasma 而不是 Xfce，因为这对我们的开发人员与 Calamares 安装程序更具本地化体验。

### 🛠️ 其他变化和改进

以下是一些值得注意的其他亮点：

  * 在新安装上启用了 **本地主机名解析**。
  * 当选择 systemd-boot 时，实施更强大的 **LUKS2 加密**。
  * 为了避免错误，对 **EFI 分区的权限** 进行了更严格的限制。
  * Calamares 上的 **软件包选择屏幕** 已经重新结构，更加直观。

你可以通过官方的 [公告博客][9] 了解更多关于 "Galileo" 发布的信息。


## 📥 获取 EndeavourOS Galileo

你可以从 [官方网站][10] 获取 EndeavourOS Galileo，他们还**在全球范围内添加了新的下载镜像**，以提高访问速度。

[EndeavourOS Galileo][10]

### 对现有用户有何影响？

没有。这个版本带来的变化仅影响新安装、安装程序和 ISO 上的实时环境。

**升级到 Galileo 不是强制性的**，定期更新系统的现有用户应该不会出现问题。

_💬 你对这个版本有什么看法？放弃 Xfce 是一个好主意吗？_

* * *

--------------------------------------------------------------------------------

via: https://news.itsfoss.com/endeavouros-galileo/

作者：[Sourav Rudra][a]
选题：[lujun9972][b]
译者：[GlassFoxowo-Dev](https://github.com/GlassFoxowo-Dev)
校对：[校对者ID](https://github.com/校对者ID)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://news.itsfoss.com/author/sourav/
[b]: https://github.com/lujun9972
[1]: https://itsfoss.com/arch-based-linux-distros/
[2]: https://news.itsfoss.com/endeavouros-cassini/
[3]: https://news.itsfoss.com/content/images/2023/11/EndeavourOS_Galileo_1.jpg
[4]: https://news.itsfoss.com/content/images/2023/11/EndeavourOS_Galileo_2.png
[5]: https://news.itsfoss.com/content/images/2023/11/EndeavourOS_Galileo_3.png
[6]: https://calamares.io/
[7]: https://github.com/EndeavourOS-Community-Editions
[8]: https://news.itsfoss.com/content/images/2023/11/EndeavourOS_Galileo_4.jpg
[9]: https://endeavouros.com/news/slimmer-options-but-lean-and-in-a-new-live-environment-galileo-has-arrived/
[10]: https://endeavouros.com/
