[#]: subject: "Top 10 Features of Linux Mint 21 “Vanessa”"
[#]: via: "https://www.debugpoint.com/linux-mint-21-features/"
[#]: author: "Arindam https://www.debugpoint.com/author/admin1/"
[#]: collector: "lkxed"
[#]: translator: "robsean"
[#]: reviewer: " "
[#]: publisher: " "
[#]: url: " "

Top 10 Features of Linux Mint 21 “Vanessa”
======
We round up the top features of the upcoming Linux Mint 21 “Vanessa”. Find out what’s in store for you.

![Linux Mint 21 Cinnamon Desktop][1]

Linux Mint 21 “Vanessa” is the 36th release of [Linux Mint][2], which carries a good list of features along with several usability improvements across the desktop. The features are scattered across the Cinnamon desktop, core changes, Xapps updates and more.

I have summarized all of them in this list of top features of Linux Mint 21.

### Top Features of Linux Mint 21 “Vanessa”

#### 1. Ubuntu 22.04 and associated updates

Perhaps the most crucial change is the base of Linux Mint 21, which is now based upon [Ubuntu 22.04 “Jammy Jellyfish”][3]. The last major release, i.e. Linux Mint 20 “Ulyana”, was based on Ubuntu 20.04 “Focal Fossa”, when released four years back. The state of the world in 2020 was utterly different, considering everything going on.

Hence, a lot of packages, version upgrades, and new performance improvements – all these under-the-hood updates come to Linux Mint 21. That includes the latest LTS [Linux Kernel 5.15][4], which brings further hardware lineup support, and toolchain updates for programming, development and networking.

#### 2. Major changes in the Timeshift backup tool

A few months back, the Mint team [announced][5] that they are taking over the development of the popular backup tool Timeshift and continuing its development as a “XApps”. So, this is a significant change. Why, may you ask?

Well, the developer of the Timeshift tool, Tony George, is busy with other projects. You may have heard about “[TeeJeeTech][6]” apps for Linux. It was created by Tony and had some cool apps. However, he doesn’t have the time to concentrate on Timeshift development and enhancement.

![Timeshift creating snapshot][7]

With that said, since Linux Mint now maintains it, some new features land in this release, such as Timeshift now determining how much disk space you need for the next backup in rsync mode (not in btrfs mode). In addition, it stops the backup process if it seems the disk space is less than 1 GB after the backup.

#### 3. WebP Support

WebP image is a reasonably new image format created by Google for the web. It beings better compression and reduced size while maintaining good quality than traditional JPEG or PNG images.

WebP support (view images, thumbnail or edit) in Linux Desktop requires some [additional installation][8] of packages. Looking at the popularity Linux Mint team brings out-of-the-box WebP support across the desktop apps and flavours.

That means Nemo file manager can show thumbnails of WebP images and view them in xviewer. The mint team always think about the end-user first because other distros are still behind on supporting WebP by default, such as Ubuntu, etc. Not only that, the new app [xapp-thumbnailers][9] now helps Nemo file manager to preview additional file types as well:

* ePub
* MP3 with Album Arts
* RAW Images
* AppImage

#### 4. Process Monitor

A small but handy tool called process monitor will give you a heads-up on what’s happening in your system. This little icon at the system tray shows up when your system is undergoing automatic updates or backup by TImeshift. In those situations, your system may become slow, and this nifty icon can show you why.

#### 5. Improved printing support

Linux Mint is well equipped for devices, and the printer supports it by default. This edition of Mint brings [Internet Printing Protocol (IPP)][10] for driverless printing and scanning.

In addition, HP’s driver, HPLIP’s latest edition (3.21.12), is also installed by default.

All these changes streamline printer and scanner usage. And users like you can enjoy effortless printing and scanning. It is such an essential aspect of a Linux distro, but it doesn’t work all the time. While [reviewing many distros][11], I found many fails to detect the printers or even print.

It’s good to see that the mint team contributed to this critical functionality.

#### 6. Window Animation updates

There are some considerable changes come in the Window and desktop animation effects. Firstly, the Effects settings for Windows and desktop are merged now. Earlier, there were separate sections which gave more granular control of the animations.

Here’s a side-by-side view.

![][12]

![][13]

Secondly, the mapping windows and desktop effects options are removed.

Third, a new control arrives to change the overall animation speed from slower to faster.

Finally, a global switch to disable or enable all the animation on the entire desktop gives you the option for more control.

I believe this is a well-designed dialog and advanced options for better clarity.

#### 7. Mutter rebase

Let’s talk about [Cinnamon desktop version 5.4][14], which comes with Linux Mint 21. It’s the latest Cinnamon release, and Mint is the first distro to bring it to the user (other than traditional Arch Linux folks, who got it [a little early][15]).

Finally, the team completed the rebase of Mutter into its window manager, Muffin in Cinnamon 5.4. Since Muffin was initially forked from Mutter, it was always lagging behind the upstream Mutter features, despite the backporting of changes. A significant amount of effort went to feature inclusion, bug fixes & clean up to make Muffin as close to the Mutter code base.

Hence, in the future, it is now easier to port back changes from Mutter upstream and clean things in Muffin as needed.

#### 8. Window manager and GTK Themes

With the changes in Muffin, the team also moved some of the display settings from gnome-control-center to cinnamon-control-center. In addition, the display configs from csd-xrandr moved into the Muffin window manager in Cinnamon 5.4. Apparently, you may not see any difference in the Display settings window. However, you may see some performance boost and fewer bugs or issues while scaling displays or in high-res windows.

Another critical change that the Mint team introduced via CInnamon 5.4 is the uniform render of GTK dialogs in apps. Earlier, if a GTK app used a header bar, then the dialog was a mix of CSD (client side decoration) and GTK themes.

Now with Cinnamon 5.4, all the windows are rendered using the GTK theme irrespective of their design. And with that, the legacy Metacity themes also dropped.

On a side note, I loved the Metacity, and its “legacy look” when [they were a thing][16] in the early days of GNOME.

#### 9. Package Management updates

Following the trends of Debian, KDE Plasma desktop, Linux Mint also protects your system from uninstalling critical dependent packages.

When you try to uninstall, Mint now checks the dependencies and whether critical desktop packages will be removed.

If found, you get an error message that stops you from going further.

On the other hand, when you successfully uninstall a package, it cleans up all the dependencies with it installed.

#### 10. Disable the Systemd OOMD (out-of-memory daemon) service

The “systemd-oomd” had some bad feedback recently since the Ubuntu 22.04 LTS release. Users across the web [reported][17] the sudden closing of applications (such as Firefox) without any warning or user intervention. Further investigation pointed to the “not so well” implementation of the systemd-oomd service.

In theory, the [systemd-oomd.service][18] monitors your system for out-of-memory situations, and it has the authority to kill any processes which consume more system resources. Ubuntu team did not communicate this with importance, which eventually led to an unpleasant user experience.

With that knowledge, Linux Mint 21 decides [not to feature][19] this service and disables it. Because the user base of Linux Mint is general users, students, etc., it would be a bad experience for users if apps closed unexpectedly.

![Systemd OOMD service is not enabled][20]

#### 11. Other Changes

Finally, let’s round up some tiny yet impactful changes to wrap up the Linux Mint 21 features.

* The default document reader app Xreader is now capable of minor annotation. This is a handy feature.
* The WebApp manager now brings custom browser parameters.
* Warpinator file transfer utility now shows you other sources on Windows, Android and iOS devices.
* Mint packages Firefox web browser as deb and not the Snap version, which defaults in Ubuntu 22.04 LTS. Thanks to Mint team, users need not worry about the [complex set of commands][21] to remove the Firefox Snap from Jammy.

![Firefox 102 in Linux Mint 21 – Exclusively packaged as deb executable][22]

* The bulk renamer app Thingy gets some UI improvements.
* The os-prober of GRUB2 is now available to detect all the operating systems in your hardware (handy for dual boot or more systems).
* The Bluetooth manager Blueman replaces Blueberry, bringing additional features for connecting and managing your Bluetooth devices.
* Finally, new wallpapers for your new desktop arrive in this release.

![New Wallpapers in Linux Mint 21][23]

### Things that are NOT changing

From a very high level, you might feel that most of the Linux Mint 21 remains the same as its predecessors. The default desktop looks and default wallpaper remains the same. Xfce and MATE desktop didn’t have any major releases. Hence they are precisely the same. In addition, the default icon theme, application menu, etc., may give you a similar feel to the entire desktop.

### Wrapping Up

Overall, a good set of features is beneficial for end users rather than being fancy gestures and stuff. For this very fact, Linux Mint is the best Linux distro today for beginners or end users. So, that concludes the feature highlights of Linux Mint 21.

The BETA testing is in progress, and there are a [few bugs reported][24]. The final release is due soon, within a few weeks from now.

You can download/update to Linux Mint 21 when released. Also, stay tuned for our detailed distro review of Linux Mint 21 after the official release.

What do you think about the new features of Linux mint 21? Is there any feature you expected but didn’t arrive in this release? Let’s discuss this in the comment box below.

--------------------------------------------------------------------------------

via: https://www.debugpoint.com/linux-mint-21-features/

作者：[Arindam][a]
选题：[lkxed][b]
译者：[译者ID](https://github.com/译者ID)
校对：[校对者ID](https://github.com/校对者ID)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://www.debugpoint.com/author/admin1/
[b]: https://github.com/lkxed
[1]: https://www.debugpoint.com/wp-content/uploads/2022/07/Linux-Mint-21-Cinnamon-Desktop.jpg
[2]: https://www.debugpoint.com/linux-mint/
[3]: https://www.debugpoint.com/web-stories/ubuntu-22-04-review/
[4]: https://www.debugpoint.com/linux-kernel-5-15/
[5]: https://blog.linuxmint.com/?p=4323
[6]: https://teejeetech.com/
[7]: https://www.debugpoint.com/wp-content/uploads/2022/07/Timeshift-creating-snapshot.jpg
[8]: https://www.debugpoint.com/view-webp-ubuntu-linux/
[9]: https://github.com/linuxmint/xapp-thumbnailers
[10]: https://datatracker.ietf.org/doc/html/rfc8011
[11]: https://www.debugpoint.com/tag/linux-distro-review/
[12]: https://www.debugpoint.com/wp-content/uploads/2022/07/Effects-in-Linux-Mint-20.jpg
[13]: https://www.debugpoint.com/wp-content/uploads/2022/07/Effects-in-Linux-Mint-21.jpg
[14]: https://github.com/linuxmint/cinnamon-desktop/releases/tag/5.4.0
[15]: https://www.debugpoint.com/cinnamon-arch-linux-install/
[16]: https://www.debugpoint.com/gnome-classic-ubuntu-22-04/
[17]: https://askubuntu.com/questions/1404888/how-do-i-disable-the-systemd-oom-process-killer-in-ubuntu-22-04
[18]: https://www.freedesktop.org/software/systemd/man/systemd-oomd.service.html
[19]: https://debugpointnews.com/linux-mint-21-systemd-oom/
[20]: https://www.debugpoint.com/wp-content/uploads/2022/07/Systemd-OOMD-service-is-not-enabled.jpg
[21]: https://www.debugpoint.com/remove-firefox-snap-ubuntu/
[22]: https://www.debugpoint.com/wp-content/uploads/2022/07/Firefox-102-in-Linux-Mint-21-Exclusively-packaged-as-deb-executable.jpg
[23]: https://www.debugpoint.com/wp-content/uploads/2022/07/New-Wallpapers-in-Linux-Mint-21.jpg
[24]: https://github.com/linuxmint/mint21-beta/issues
