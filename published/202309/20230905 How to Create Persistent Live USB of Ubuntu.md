[#]: subject: "How to Create Persistent Live USB of Ubuntu"
[#]: via: "https://itsfoss.com/ubuntu-persistent-live-usb/"
[#]: author: "Sagar Sharma https://itsfoss.com/author/sagar/"
[#]: collector: "lujun9972/lctt-scripts-1693450080"
[#]: translator: "ChatGPT"
[#]: reviewer: "wxy"
[#]: publisher: "wxy"
[#]: url: "https://linux.cn/article-16165-1.html"

如何创建 Ubuntu 持久化立付 U 盘
======

![][0]

> 体验带有持久化的立付 U 盘，你在立付会话中做出的所有改动都会被保存。在此教程中，你将学习如何创建一个持久化的 U 盘。

如果我告诉你，你能将完整的 Ubuntu 系统装载在一个可移动的 U 盘上，你会有何感想？

在外置 U 盘上 [安装 Ubuntu][1] 过程相当复杂。一种更容易的方法是制作一个带有持久化存储的 <ruby>立付<rt>Live</rt></ruby> U 盘，这样你对 U 盘做出的改动都会被保存下来。

请相信我，这个过程跟使用 [BalenaEtcher][2] 或其他任何刻录工具创建可引导驱动器的过程十分相似。

然而，我们在开始之前，让我们先弄清楚持久化立付 U 盘是什么。

### 什么是持久化立付 U 盘？

当你使用立付 Linux U 盘时，你在 <ruby>立付会话<rt>Live session</rt></ruby> 中做出的所有更改，在重启以后都将丢失。比如，你必须重新连接 Wi-Fi，并且你下载的文件及安装的应用均不会被保留。而持久化立付 U 盘将会为你保存这些所有的更改。

这样，你就可以将该 U 盘作为一个外置操作系统使用，它将会保存你所做出的所有更改，比如创建用户账号，安装软件包，和一切你通常在电脑上做的事情。

当然，保存的文件数量将取决于你使用的 U 盘的大小！

但你已经明白我要表达的意思了吧。那么，我们开始学习如何创建一个带有持久性的 Ubuntu 立付 U 盘吧。

### 如何创建一个持久化的 Ubuntu U 盘

在这个教程中，我将引导你完成一个持久化的 Ubuntu U 盘的制作过程：

  * 通过在 Windows 上的 Rufus 工具
  * 或者，通过在 Linux 上的 mkusb 工具

你可以参照教程中的适合你的部分。

> 📋 本教程中，你将会创建一个 Ubuntu 的持久化 U 盘。并非所有的 Linux 发行版都支持数据的持久化存储，所以这个方法可能并非所有的发行版本适用。

### 方法 1：在 Windows 上创建持久化的 Ubuntu U 盘

在 Windows 上创建一个持久化的 Ubuntu U 盘，我会使用 Rufus，这是一款自由开源工具，专门用于将 ISO 文件刻录到 U 盘上。

请访问 [Rufus 的官方下载页面][3]，获取 Windows 版本的可执行文件：

![][4]

然后，打开 Rufus，它将要求以管理员身份运行；请授予该权限，因为你即将在外部驱动器上做改动，需要相应的权限。

接下来，根据以下步骤使用 Rufus 创建持久化 U 盘：

  * 选中 U 盘设备（如果只有一个 U 盘，它将默认被选中）。
  * 点击 “<ruby>选择<rt>Select</rt></ruby>” 按钮，在文件管理器中选择 ISO 文件。
  * 你可以使用滑块或直接设定持久化分区的大小（可以放心地设定为最大值）。
  * 其他选项保持默认设置（除非你清楚在做什么）。
  * 点击 “<ruby>开始<rt>Start</rt></ruby>” 按钮，开始进行刻录。

![][5]

该程序你会告诉你，选中的驱动器上的所有数据将会被删除，所以你可以放心忽略这个警告。

完成后，我们可以来瞧瞧如何在 Windows 中直接启动到 UEFI 设置。

#### 通过 U 盘启动（简化版） 

这个方法应适用于大多数用户，如果无效，你总是可以选择传统的方式，那就是重新启动系统并按下 `Esc`、`Delete`、`F1`、`F2`、`F10`、`F11` 或 `F12` 等按键。

步骤如下：按 `Win + X`，然后以管理员身份启动 Windows PowerShell：

![][6]

一旦你看见提示符，直接运行以下命令：

```
shutdown.exe /r /fw
```

这将会计划一个关机动作，稍后，你会进入到 UEFI 固件设置。

到了这步，选择 U 盘作为首选的启动选项并保存设置：

![][7]

你会看到一个正常的 GRUB 屏幕：

![][8]

当你启动后，选择试用 Ubuntu 的选项，然后你所做的任何改动都可以被保存下来，即使你重新启动了电脑也无所谓。

### 方法 2：在 Ubuntu Linux 上创建持久化 Ubuntu U 盘

> 🚧 请注意，这种方法主要适用于 Ubuntu 和 Debian 的 ISO。

如果你还不知道，`mkusb` 是一个带有 GUI 的工具，让你能够将 ISO 文件刷到磁盘驱动器上，并且有附加功能，例如在 Ubuntu 上创建持久化驱动器。

你需要添加 `mkusb` 的 PPA 来进行安装，具体命令如下：

```
sudo add-apt-repository ppa:mkusb/ppa
```

要使改变生效，需要更新软件库索引：

```
sudo apt update
```

最后，安装 `mkusb` 以及其他相关软件包：

```
sudo apt install --install-recommends mkusb mkusb-nox usb-pack-efi
```

就这样！

首先，从系统菜单启动 `mkusb` 工具，它会提示你输入超级用户密码：

![][9]

操作完成后，它会提示你所有驱动器上的数据将会被新数据覆盖。

只需简单地点击 “OK” 按钮即可：

![][10]

然后它会显示 `mkusb` 工具能执行的多项操作，你需要选择第一选项 “<ruby>安装（制作一个启动设备）<rt>Install (make a boot device)</rt></ruby>”：

![][11]

接下来，它会显示许多安装选项，你需要选择第三个选项 “<ruby>持久化立付（仅针对 Debian 和 Ubuntu）<rt>'Persistent live' - only Debian and Ubuntu</rt></ruby>”：

![][12]

在下一个步骤中，它会让你在多种方法/工具中选择一个，如果没有使用特定类型的版本，例如超精简版本，建议使用第一个名为 “dus-Iso2usb” 的方法：

![][13]

接着，它会让你从文件管理器中选择你需要的 ISO 文件：

![][14]

工具会显示已选 ISO 文件的名称，以及创建持久化 U 盘所要使用的工具：

![][15]

下一步，你需要选择驱动器将之前选择的 ISO 文件刷入：

![][16]

以上全部完成后，将会有 3 个选项供你选择。如果你不确定使用哪一个，那么就点击 “<ruby>使用默认<rt>Use defaults</rt></ruby>” 按钮，但是大多数用户选择第二个选项 “grold” 即可（我也是选择这个）：

![][17]

检查一切都无误后，点击 “<ruby>开始<rt>Go</rt></ruby>” 开始刷新过程：

![][18]

现在，刷入过程已经开始了！

![][19]

**注意，这个刷入过程会比你使用 BalenaEtcher 刷入要长一些时间！**

完成后，会有通知告诉你，过程已经完成，此时你可以取下 U 盘，然后重新插上，以查看更改的内容：

![][20]

#### 从持久化 U 盘启动

如果你要从 U 盘启动，通常可以重启你的系统，连续按下对应的按钮即可，但这已经是旧方法了！

在 Linux 中，有一种更为简便的方式访问 BIOS，你只需在终端执行以下命令：

```
systemctl reboot --firmware-setup
```

然后，进入启动菜单并将 U 盘设置为首选的启动选项：

![][22]

一旦你从 U 盘启动，你将有两个选项：

  * 带有持久化模式的 ISO
  * 以实时模式进行启动

如其名，你需要选择第一个选项以启动进入 Ubuntu 的持久化模式：

![][23]

现在，你可以进行各种修改，如安装你喜欢的软件包，[创建新用户][24] 等等！

我希望这个指南对你有所帮助。

*（题图：MJ/423c72d6-d6eb-4146-acd5-1e58eed11f41）*

--------------------------------------------------------------------------------

via: https://itsfoss.com/ubuntu-persistent-live-usb/

作者：[Sagar Sharma][a]
选题：[lujun9972][b]
译者：ChatGPT
校对：[wxy](https://github.com/wxy)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://itsfoss.com/author/sagar/
[b]: https://github.com/lujun9972
[1]: https://itsfoss.com/intsall-ubuntu-on-usb/
[2]: https://itsfoss.com/install-etcher-linux/
[3]: https://rufus.ie/en/
[4]: https://itsfoss.com/content/images/2023/09/Download-Rufus-to-create-persistant-Ubuntu-drive-in-Windows.png
[5]: https://itsfoss.com/content/images/2023/09/Use-rufus-to-create-Ubuntu-persistant-drive.png
[6]: https://itsfoss.com/content/images/2023/09/Start-Windows-powershell-as-admin.png
[7]: https://itsfoss.com/content/images/2023/09/Boot-from-UEFI-1.jpg
[8]: https://itsfoss.com/content/images/2023/09/Boot-from-persisted-storage-USB-drive-made-using-Rufus-on-Windows-machine.png
[9]: https://itsfoss.com/content/images/2023/08/Start-mkusb-tool-from-system-menu.png
[10]: https://itsfoss.com/content/images/2023/08/Data-will-be-wiped-warning-.png
[11]: https://itsfoss.com/content/images/2023/08/Select-the-first-option-in-mkusb-tool-to-create-persistent-USB-drive-of-Ubuntu.png
[12]: https://itsfoss.com/content/images/2023/08/Select-the-persistent-option.png
[13]: https://itsfoss.com/content/images/2023/08/Select-the-grub-option.png
[14]: https://itsfoss.com/content/images/2023/08/Select-an-ISO-file-to-create-persistent-USB-from-Ubuntu.png
[15]: https://itsfoss.com/content/images/2023/08/Showing-seelcted-ISO-file.png
[16]: https://itsfoss.com/content/images/2023/08/Choose-drive-to-create-persistent-drive.png
[17]: https://itsfoss.com/content/images/2023/08/Choose-bootloader.png
[18]: https://itsfoss.com/content/images/2023/08/Select-go-ahead-option-in-mkusb-to-create-persistent-USB-drive.png
[19]: https://itsfoss.com/content/images/2023/08/Flashing-process-to-make-persistent-usb-of-Ubuntu.png
[20]: https://itsfoss.com/content/images/2023/08/Persistent-drive-has-been-made.png
[21]: https://itsfoss.com/access-uefi-from-linux/
[22]: https://itsfoss.com/content/images/2023/09/Boot-from-UEFI.jpg
[23]: https://itsfoss.com/content/images/2023/08/Boot-from-persisted-storage-USB-drive.png
[24]: https://learnubuntu.com/add-delete-users/
[25]: https://itsfoss.com/content/images/size/w256h256/2022/12/android-chrome-192x192.png
[0]: https://img.linux.net.cn/data/attachment/album/202309/06/162606ivjl1zoohb1h8vuo.jpg