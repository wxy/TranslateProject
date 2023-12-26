[#]: subject: "11 Fish Shell Features That Make it More Awesome Than Bash"
[#]: via: "https://itsfoss.com/fish-shell-features/"
[#]: author: "Abhishek Prakash https://itsfoss.com/author/abhishek/"
[#]: collector: "lujun9972/lctt-scripts-1700446145"
[#]: translator: "ChatGPT"
[#]: reviewer: "wxy"
[#]: publisher: "wxy"
[#]: url: "https://linux.cn/article-16504-1.html"

让 Fish Shell 比 Bash 更好的 11 大特性
======

![][0]

> 就算你是素食主义者或对海鲜有过敏反应，也值得试试 Fish :P

Bash 是使用最广泛的 Shell，Zsh 则是开发者圈里最受青睐的，但 Fish 往往被许多人忽视。

这绝非夸张之辞。Fish 的确是个备受忽视的 Shell，它对新手和资深的自由开源软件用户，都可能是极好的选择。

Fish 提供了一系列吸引人的功能，使其具有鲜明优势。这其中包括了从语法高亮到缩写（我个人最喜欢的部分），这里面充满了种种新奇。

下面，我要和大家分享一些我最青睐的 Fish Shell 特性。

### 1、语法高亮

在错误的命令被执行之前就识别出它们将大大节省你的时间，同时降低你的挫败感。

现代的许多代码编辑器都内置了语法高亮功能，而 Fish 不仅将此功能内置在了 Shell 中，而且对于 Linux 命令也同样有效。

命令有误？你会发现其被红色高亮。同样的，对于不符合上下文的参数和选项也是如此。

![错误高亮为红色][1]

### 2、自动建议

当你输入命令时，Fish Shell 会自动推荐命令，然后你可以按照提示，使用 `Tab` 键进行相应的补全操作。

![Fish 自动补全][2]

随着你的输入，建议会以灰色显示，使其更易于识别。如果整条建议都对你的胃口，你可以**按右箭头键来完成整个命令的补全**。

### 3、命令选项的交互式手册页

这是一个炫酷的功能，你可以交互性地参考手册页完成命令选项的填写。

首先，你需要先解析手册页，这可以通过以下命令来完成：

```
fish_update_completions
```

这会对手册页进行解析。

![手册页解析][3]

现在，如果你输入一个命令，添加连字符作为选项，然后按下 `Tab` 键，就能看到手册页给出的可能选项及其简短描述：

![Fish 手册页帮助][4]

你可以通过滚动一览这些选项，并在阅读了作用说明后，从弹出的分页器中进行选择。

要比直接输入 `command -h` 更便利一些对吧。

### 4、缩写优于别名

在 Fish 里，缩写的作用就如同文本扩展工具。你可以为一些常用的代码设置易于调用的缩写。

比如说，我把 `sch` 设为 `pacman -Ss` 的缩写，用以搜索软件包。

```
abbr -a sch pacman -Ss
```

于是，每次我输入 `sch` 并按空格键后，它就会被替换成 `pacman -Ss`。

![Fish Shell 缩写][5]

你甚至可以把它写入配置文件，让其成为永久设置。

> 💡 别名和缩写的关键区别在于，别名的工作是内部完成的，你看不到其背后真正运行的命令。而缩写不仅会展示实际的命令，而且会让它们在历史记录里也正确地出现。

### 5、丰富的基于 Web 的帮助

Linux 纯粹主义者常常依赖手册页来寻求命令帮助，而新一代的 Linux 用户则更多地依赖网络资源。

Fish 则结合了这两者优点，提供了详尽的“基于 Web 的帮助”功能，并且且易于使用，即便在无网络连接的情况下也同样可用，因为它是本地化存储的。

在运行 Fish Shell 时，仅需输入：

```
help
```

就可以在你的网络浏览器上打开帮助页面了。

![Fish Shell 网页帮助][6]

如今，你可以随时方便地查阅这份详细的文档。

### 6、基于 Web 的配置

没错，这是另一个“基于 Web”的功能。

要改变提示符颜色或其他配置，你不必在终端里编辑配置文件，相反地，你可以运行基于 Web 的配置。

在运行 Fish Shell 时，只需输入以下命令：

```
fish_config
```

这会打开你的浏览器，并显示出配置设置。

![Fish Shell 基于 Web 的配置][7]

在这里，你可以更改颜色，从现有列表中选择一个不同的提示符等等。

![提示符选择][8]

通过这种方式来改变配置更方便，对吗？

### 7、自动切换目录

如果你想切换到某个目录，你不需要输入 `cd` 命令。只需要键入该目录名称就行了。

例如，如果你位于主目录，并希望切换到 `Downloads` 目录，只需要输入 `Downloads`。输入过程中，它会进一步给出补全建议。

![自动 cd][9]

如果你正在某个特定目录中，想要跳转到一个完全不同的路径，则需要使用绝对路径。

### 8、更简洁的路径导航

如果你需要在=浏览过的目录之间来回切换，没必要输入路径或使用 `cd ..` 等。只要**按 `ALT + ←` 或 `ALT + →`，分别向前和向后移动**就行了。

![目录导航][10]

或者，你可以键入 `cdh` 并按回车，这会呼出一个分页器界面，你可以使用对应的数字来回到你想去的目录。

![使用分页器导航][11]

### 9、交互式历史搜索

你可以在 Fish 中交互式地搜索某个特定的历史命令。做这个的时候，就使用我们熟悉的 `CTRL+R` 就行了。

这会呼出一个类似于分页器的界面，显示一个搜索提示。输入你想要查找的命令，就能看到搜索结果：

![交互式历史搜索][12]

### 10、全局变量

在 Fish Shell 中，如果你将一个变量设置为全局的，那么它将在重启 Shell 或者重启系统后仍然可用。

要设置一个全局变量，可以使用：

```
set -U my_variable 10
```

这时，`my_variable` 的值将会被设置为 10，即使系统重启后也不变。

是的，不需要将它们添加到你的 RC 或 profile 中。

### 11、隐私模式

Fish Shell 有一个隐私模式，该模式下输入的命令将不会被保存到历史记录或存储在硬盘上。

要进入隐私模式，使用命令：

```
fish -P
```

![Fish 隐私模式][13]

工作完成后，通过键入 `exit` 就可以退出隐私模式。

### Fish 还有更多你可以探索的

[Fish Shell][15] 提供了许多其他的用户友好特性，比如：

  * 使用 `ALT+Enter` 实现简单的多行命令编辑
  * 切换 Emacs（默认）/Vim 键位绑定
  * 提供简洁明了的脚本编写语法

当然，你可以在其他 Shell 中通过一些努力实现大部分 Fish Shell 的特性，但默认启用这些特性可就完全是另一回事了。

Fish 可以帮助你在掌控开发环境的前提下，提高开发工作的效率。别把为 Fish Shell 编写脚本运行在 Bash 中，在多用户系统的共享环境中可能会引发 Shell 兼容性问题。

如果你喜欢这些特性，试试 Fish Shell 看看效果如何。也许你会将 Fish 设为 [你的默认 Shell][16]。

即使你不想在终端里看到 “Fish”，也许你会喜欢 ASCII 水族馆 😉

> **[在 Linux 终端利用 Asciiquarium 打造海底世界][14]**

💬 请在评论中分享你对 Fish Shell 的看法 😄

*（题图：DA/8522d28f-40ab-4eaa-b2b5-bc627f114224）*

--------------------------------------------------------------------------------

via: https://itsfoss.com/fish-shell-features/

作者：[Abhishek Prakash][a]
选题：[lujun9972][b]
译者：[ChatGPT](https://linux.cn/lctt/ChatGPT)
校对：[wxy](https://github.com/wxy)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://itsfoss.com/author/abhishek/
[b]: https://github.com/lujun9972
[1]: https://itsfoss.com/content/images/2023/12/Error-in-red-color.png
[2]: https://itsfoss.com/content/images/2023/12/fish-auto-completion.svg
[3]: https://itsfoss.com/content/images/2023/12/fish-update-completions.png
[4]: https://itsfoss.com/content/images/2023/12/fish-man-page-completion.svg
[5]: https://itsfoss.com/content/images/2023/12/fish-abbr-examples.svg
[6]: https://itsfoss.com/content/images/2023/12/fish-web-help.png
[7]: https://itsfoss.com/content/images/2023/12/fish-web-configuration.png
[8]: https://itsfoss.com/content/images/2023/12/fish-various-prompts.png
[9]: https://itsfoss.com/content/images/2023/12/fish-automatic-cd.svg
[10]: https://itsfoss.com/content/images/2023/12/fish-navigation.svg
[11]: https://itsfoss.com/content/images/2023/12/fish-navigation-cdh.svg
[12]: https://itsfoss.com/content/images/2023/12/fish-interactive-history.svg
[13]: https://itsfoss.com/content/images/2023/12/fish-private-mode.svg
[14]: https://linux.cn/article-16354-1.html
[15]: https://fishshell.com/
[16]: https://itsfoss.com/linux-change-default-shell/
[0]: https://img.linux.net.cn/data/attachment/album/202312/25/183053z4974f7g0077az6i.jpg