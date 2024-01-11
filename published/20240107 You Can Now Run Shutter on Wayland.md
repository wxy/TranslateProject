[#]: subject: "You Can Now Run Shutter on Wayland!"
[#]: via: "https://news.itsfoss.com/shutter-wayland-linux/"
[#]: author: "Sourav Rudra https://news.itsfoss.com/author/sourav/"
[#]: collector: "lujun9972/lctt-scripts-1700446145"
[#]: translator: "ChatGPT"
[#]: reviewer: "wxy"
[#]: publisher: "wxy"
[#]: url: "https://linux.cn/article-16549-1.html"

现在你可以在 Wayland 上运行 Shutter 了！
======

![][0]

> 你无需在 Wayland 上放弃使用 Shutter！

哎，我一直在担心有一天我得切换到只支持 Wayland 的 Linux 发行版，结果发现 [Shutter][1] 不工作。

它是 Linux 中用于捕捉和编辑 [屏幕截图的最佳工具][2] 之一，我每天都会使用它来为这里和其他地方的工作捕捉各种截图。

我知道 GNOME 的屏幕截图工具已经有了很大的进步，但是就像人们所说的，“旧习难改”。所以，当我发现有一种方法可以在所有的 Wayland 上运行 Shutter 时，我自然是相当兴奋。

请跟随我一起了解这个精彩的开源项目。这个项目由一位热心的 Shutter 爱好者发起，他的目标就是让 Shutter 能在配备 Wayland 的发行版上顺利运行。

### 在 Wayland 上使用 Shutter：有何期待？

这个项目由来自意大利的 IT 开发者 Maurizio 发起，他热衷于 Linux，**因为他不能接受 Shutter 无法在他的 Ubuntu 系统上正常运行，因此这个项目应运而生。**。

因此，他复刻了 Shutter 的代码仓库，并利用 [GNOME 的屏幕截图工具][4] 的命令行工具进行开发，同时**尽力保持用户界面和以往的操作习惯不变**。

如下图所示，这个项目**与你从 Shutter 那里期待的体验几乎无二**，你可以在界面上发现所有熟悉的选项。在运行着 Ubuntu 23.10 的虚拟机上用这个工具截图时，我并未感到有什么两样。

![][5]

我还发现，**按只截图窗口或选取特定区域也变得容易了**。只是那个通常用来截图特定窗口或桌面的下拉菜单似乎并未起到应有的功能，反而变得有点挪作他用。

> 📋 这是我在 Ubuntu 23.10 的 Wayland 上进行选区捕捉的结果。

![][6]

如果你想截图你系统中特定的桌面空间，你需要切换到那个桌面，使 Shutter 转到同一屏幕，然后使用“<ruby>桌面<rt>Desktop</rt></ruby>”选项进行截图。

![][7]

对于只截图窗口也是类似，只要将应用和 Shutter 切到同一屏幕，使用“<ruby>窗口<rt>Window</rt></ruby>”选项就能够截取窗口的截图。

**至此已经足够了**。我真心期待 Shutter 的开发更上层楼，希望我们能看到此类改进被融入原有的项目中。

### 📥 如何下载运行于 Wayland 的 Shutter?

在开始下载和安装之前，请确保你已经彻底卸载了你之前安装的任何版本的 Shutter。

接下来，你有两种获取这个 Shutter 变体的方法可选。第一种方法是直接访问它的 [GitHub 仓库][8]，下载提供的 “.deb” 文件。

> **[在 Wayland 上的 Shutter（GitHub）][9]**

而我更为推荐的是第二种方法，尤其适用于 **Ubuntu 23.10 或者更高的版本**，因为它可以自动处理所有的依赖关系。你只需要运行以下的命令即可：

```
setfacl -m u:_apt:rx .
wget https://github.com/mvivarelli/shutter-on-wayland/raw/master/shutter-on-wayland_0.99.4-6_all.deb
sudo apt -f install ./shutter-on-wayland_0.99.4-6_all.deb
```

如果安装后你在启动 Shutter 时遇到了卡顿或者延迟的问题，那么你可以通过重启你的系统来解决此类问题。

💬 对于这个项目，你有什么样的想法呢？你会考虑使用它吗？

--------------------------------------------------------------------------------

via: https://news.itsfoss.com/shutter-wayland-linux/

作者：[Sourav Rudra][a]
选题：[lujun9972][b]
译者：[ChatGPT](https://linux.cn/lctt/ChatGPT)
校对：[wxy](https://github.com/wxy)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://news.itsfoss.com/author/sourav/
[b]: https://github.com/lujun9972
[1]: https://shutter-project.org/
[2]: https://itsfoss.com/take-screenshot-linux/
[3]: https://itsfoss.com/content/images/size/w256h256/2022/12/android-chrome-192x192.png
[4]: https://gitlab.gnome.org/GNOME/gnome-screenshot
[5]: https://news.itsfoss.com/content/images/2024/01/Shutter_on_Wayland_1-1.png
[6]: https://news.itsfoss.com/content/images/2024/01/Shutter_on_Wayland_2-1.png
[7]: https://news.itsfoss.com/content/images/2024/01/Shutter_on_Wayland_3.png
[8]: https://github.com/mvivarelli/shutter-on-wayland/tree/master
[9]: https://github.com/mvivarelli/shutter-on-wayland/blob/master/shutter-on-wayland_0.99.4-6_all.deb
[0]: https://img.linux.net.cn/data/attachment/album/202401/11/073858ajzm1eef77me0fgz.jpg