[#]: subject: "AUR Helper Paru 2.0 Upgrade is Here With Features for Power Users"
[#]: via: "https://news.itsfoss.com/aur-helper-paru-2-0/"
[#]: author: "Sourav Rudra https://news.itsfoss.com/author/sourav/"
[#]: collector: "lujun9972/lctt-scripts-1700446145"
[#]: translator: "ChatGPT"
[#]: reviewer: "wxy"
[#]: publisher: "wxy"
[#]: url: "https://linux.cn/article-16433-1.html"

Paru 2.0 版本升级，为高级用户带来了新特性
======

![][0]

> 经过了一段时间的等待，Paru 2.0 版本终于发布了。

如果你不熟悉 Paru，它其实是一个 [AUR 帮助程序][1]，可以自动完成手动构建 [PKGBUILD][2] 的过程，方便在 Arch Linux 中安装软件包。

现新版 Paru 2.0 正式发布，此次更新中包含了一些重要的改进。

不过在深入了解之前，你需要确保自己知道如何解决在使用 AUR 帮助程序构建软件包时可能遇到的问题。如果你刚接触 Linux，我们建议你坚持使用你熟悉的包管理器。

### 🆕 Paru 2.0: 有什么新变化？

![][3]

Paru 2.0 版本是一次重大更新，目标是带来一些主要的改变，尤其是为了满足高级用户的需求。

该版本距离上个重大版本的发布已经过去了一年多。开发者表示由于时间不足，需要完成的改变还有很多。

由于很长一段时间没有发布版本，所以开发者提到了这个版本的很多内容都没有经过严格的测试，可能随后会发布 .1 补丁。

现在，我们来看看 Paru 2.0 版本的重要改进点。

首先，现在你可以把非 AUR 的 `PKGBUILD` 集成到构建引擎中。你可以在你的 `paru.conf` 中加入其他的 pkgbuild 仓库，具体命令如下：

```
[repo_name]
Url = https://path/to/git/repo
```

然后运行下列命令，同步这个新加入的仓库：

```
paru -Sy --pkgbuilds
```

此外，你还可以指定一个本地路径，指向你的本地 pkgbuild 仓库。

这些新加入的仓库比 AUR 具有优先级，并且它们还允许包含 AUR 的依赖项。

而新加入的另一项特性就是一个名为 `.` 的新的自动 pkgbuild 仓库，这个新的仓库在 `paru.conf` 中是无法看到的。

这个新的特性允许执行 `paru -S ./foo` 命令，其中 `foo` 是当前目录下的某个包的名字。

这样你就能在同一个目录中管理一系列相互依赖的 pkgbuild，通过上面的命令，你可以构建其中任何一个pkgbuild。

当你开始构建它们时，Paru 将会自动解决和构建该路径下的 pkgbuild 包的依赖问题。

#### 🛠️ 其他的改变和优化

除了上述的改变，本次更新还带来了其他一些变动：

  * 修复了在运行 `paru -Sc` 时没有 sudo 的问题。
  * 日期现在会显示为你的系统的本地时区。
  * 改进了搜索功能，现在默认是启用状态。
  * 在最后的 Paru 确认后，无需再额外对 pacman 确认安装。
  * `--chroot` 现在无需本地的仓库，当然，如果有的话它会工作得更好。

对于这个版本的更深入的了解，你可以参阅 [发布说明][4]。

### 📥 获取 Paru 2.0

如果你是从 AUR 安装的 Paru，你可以直接在 AUR 中升级到 2.0 版本。但如果你是自己构建的 Paru ，那可以试试使用 `-U` 命令进行更新，或者重新构建一次。

如果你是第一次安装 Paru ，你可以前往其 [GitHub 仓库][5] ，按照里面的安装说明操作就可以了。

> **[Paru 2.0（GitHub）][4]**

如果你想要了解更多关于 Paru 的信息，或者想学习如何安装 Paru，我强烈建议你浏览我们关于 [Paru AUR 帮助程序][6] 的文章：

> **[Paru - 基于 Yay 的 AUR 助手和 Pacman 封装器][6]**

💬 Arch 用户，你对这次的 Paru 版本升级感到兴奋吗？分享一下你的想法吧！

--------------------------------------------------------------------------------

via: https://news.itsfoss.com/aur-helper-paru-2-0/

作者：[Sourav Rudra][a]
选题：[lujun9972][b]
译者：[ChatGPT](https://linux.cn/lctt/ChatGPT)
校对：[wxy](https://github.com/wxy)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://news.itsfoss.com/author/sourav/
[b]: https://github.com/lujun9972
[1]: https://wiki.archlinux.org/title/AUR_helpers
[2]: https://wiki.archlinux.org/title/PKGBUILD
[3]: https://news.itsfoss.com/content/images/2023/11/Paru_2.0.png
[4]: https://github.com/Morganamilo/paru/releases/tag/v2.0.0
[5]: https://github.com/Morganamilo/paru/
[6]: https://itsfoss.com/paru-aur-helper/
[7]: https://itsfoss.com/content/images/size/w256h256/2022/12/android-chrome-192x192.png
[0]: https://img.linux.net.cn/data/attachment/album/202312/01/224300e5sire0nczj55sc8.jpg