[#]: subject: "Customize GNOME 42 with A Polished Look"
[#]: via: "https://www.debugpoint.com/2022/05/customize-gnome-42-look-1/"
[#]: author: "Arindam https://www.debugpoint.com/author/admin1/"
[#]: collector: "lkxed"
[#]: translator: "geekpi"
[#]: reviewer: " "
[#]: publisher: " "
[#]: url: " "

Customize GNOME 42 with A Polished Look
======
A tutorial on how you can give your favourite GNOME desktop a polished look, in 5 minutes.

There are many ways you can customize your favourite GNOME desktop with icons, themes, cursors and wallpapers. This article shows you how to give the GNOME 42 desktop a more polished look. The GNOME 42 desktop environment is available with the recently released Ubuntu 22.04 LTS and Fedora 36.

Before you read further, here’s how it looks with a side by side comparison (before and after).

![GNOME before customisation][1]

![GNOME after customisation][2]

I am going to divide this tutorial into two sections.

The first section deals with setting up and installing required packages. And second, how to apply various settings to get your desired look.

This tutorial was mainly tested on Ubuntu 22.04 LTS. However, it should work in other variants of Ubuntu and Fedora.

### Customize GNOME 42 with a Polished Look

#### Setup

* First, enable your system for Flatpak because we need to install the Extension Manager to download some required GNOME Shell extensions for this tutorial.

* So, to do that, open up a terminal and run the following commands.

```
sudo apt install flatpak gnome-software-plugin-flatpakflatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

* Reboot the computer once done.

* Then run the following command from the terminal to install the Extensions Manager app to download GNOME Shell Extensions.

```
flatpak install flathub com.mattjakeman.ExtensionManager
```

* Open the Extension Manager application and install two extensions. The first one is Floating Dock which features a super cool dock which you can move around anywhere on your desktop. Second, install the User themes extensions to help you install the external GTK themes in your Ubuntu Linux.

![User Themes Extension][3]

![Floating Dock Extension][4]

* Secondly, install the [Materia Theme][5] using the below commands. You have to build it as it doesn’t have any executable. Run the following commands in sequence in Ubuntu to install.

```
git clone https://github.com/ckissane/materia-theme-transparent.gitcd materia-theme-transparentmeson _buildmeson install -C _build
```

* Additionally, download the [Kora Icon theme][6] from the below link. After downloading, extract the files and copy the below four folders to `/home/<user name>/.icons` path. Create the .icons folder if it is not present.

[Download Kora Icon Theme][7]

![Kora Icon Theme][8]

* Besides the above changes, download the awesome Bibata cursor theme from the below link. After download, extract and copy the folders to the same `/home/<user name>/.icons` folder.

[Download Bibata Cursor Theme][9]

* In addition to the above, if you want a nice font which goes with the above themes, [download Robot font][10] from Google Fonts and copy them to `/home/<user name>/.fonts` folder.

* Finally, restart your system once again.

#### Configuration

* Open the Extension Manager, enable the Floating Dock and User Themes, and disable the Ubuntu Dock.

![Changes to Extensions][11]

* In addition, open the Floating dock settings and make the following changes.

![Floating Dock Settings][12]

* Furthermore, open the [GNOME Tweak Tool][13], and go to the Appearance tab. Set the followings.Cursor: Bibata-Original-IceShell Theme: MateriaIcon: Kora
* Cursor: Bibata-Original-Ice
* Shell Theme: Materia
* Icon: Kora

* Cursor: Bibata-Original-Ice
* Shell Theme: Materia
* Icon: Kora

* Other than that, you may also want to change the font. To do that, go to the Fonts tab and change the document and interface to Robot 10pt.

* Alternatively, you can also change the accent colour and style from Settings which comes by default with Ubuntu 22.04.

* Finally, download a nice wallpaper as per your preference. For this tutorial, I have downloaded a sample wallpaper from [here][14].

* If all goes well, you should have a nice desktop, as shown below.

![Customize GNOME 42 – Final Look][15]

Enjoy a polished GNOME 42. Cheers.

--------------------------------------------------------------------------------

via: https://www.debugpoint.com/2022/05/customize-gnome-42-look-1/

作者：[Arindam][a]
选题：[lkxed][b]
译者：[译者ID](https://github.com/译者ID)
校对：[校对者ID](https://github.com/校对者ID)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://www.debugpoint.com/author/admin1/
[b]: https://github.com/lkxed
[1]: https://i2.wp.com/www.debugpoint.com/wp-content/uploads/2022/05/GNOME-before-customisation.jpg?ssl=1
[2]: https://i0.wp.com/www.debugpoint.com/wp-content/uploads/2022/05/GNOME-after-customisation.jpg?ssl=1
[3]: https://www.debugpoint.com/wp-content/uploads/2022/05/User-Themes-Extension2.jpg
[4]: https://www.debugpoint.com/wp-content/uploads/2022/05/Floating-Doc-Extension.jpg
[5]: https://github.com/ckissane/materia-theme-transparent
[6]: https://github.com/bikass/kora/
[7]: https://github.com/bikass/kora/archive/refs/heads/master.zip
[8]: https://www.debugpoint.com/wp-content/uploads/2022/05/Kora-Icon-Theme.jpg
[9]: https://www.pling.com/p/1197198/
[10]: https://fonts.google.com/specimen/Roboto
[11]: https://www.debugpoint.com/wp-content/uploads/2022/05/Changes-to-Extensions.jpg
[12]: https://www.debugpoint.com/wp-content/uploads/2022/05/Floating-Dock-Settings.jpg
[13]: https://www.debugpoint.com/2018/05/customize-your-ubuntu-desktop-using-gnome-tweak/
[14]: https://www.pexels.com/photo/colorful-blurred-image-6985048/
[15]: https://www.debugpoint.com/wp-content/uploads/2022/05/Customize-GNOME-42-Final-Look.jpg
