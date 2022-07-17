[#]: subject: "Guide: How to Share A Folder Between Ubuntu/Linux and Windows"
[#]: via: "https://www.debugpoint.com/guide-how-share-folder-between-ubuntu-linux-windows/"
[#]: author: "Arindam https://www.debugpoint.com/author/admin1/"
[#]: collector: "lkxed"
[#]: translator: "MjSeven"
[#]: reviewer: " "
[#]: publisher: " "
[#]: url: " "

Guide: How to Share A Folder Between Ubuntu/Linux and Windows
======
This beginner’s guide explains how you can quickly share a folder in Ubuntu/Linux.

Sharing a folder in Ubuntu/Linux and accessing the same over the network in other OS such as Windows is not that difficult. To perform this, the required packages are not installed by default in Ubuntu. However, you can bring up the install wizard to install the required software automatically to share a folder.

This [guide][1]applies to all Ubuntu versions (including [22.04][2], 20.04, 18.04, 19.10 and upcoming – unless there are major changes in how this function is designed).

### Steps to Share a Folder in Ubuntu

**Step 1:** Open the file manager and right-click on the folder you want to share. Click on the option “Local Network Share” in the context menu.

![Local Network Share Option][3]

**Step 2:** Click on the Share this folder checkbox in the Folder Sharing dialog.

This would install [Samba][4]packages in your system. Samba is used to share files and printers over the network between Windows and Unix systems.

![Folder Sharing Option - Install Samba][5]

**Step 3:** After samba installation, do the following to share a folder or directory.

* Select the checkbox Share this folder.
* Input a share name. This would be the name you would be seeing from another system, e.g. Windows. Try not to use any name with spaces.
* (Optional) You can control the write permission to the shared folder and allow guest access by checking the corresponding option.
* If you allow guest access, people without credentials can access the shared folder. So be cautious.
* If you want your users to enter their usernames and password, open the terminal and run the below command.

```
sudo smbpasswd -a Username
```

**username** should be a valid user of the respective Ubuntu system.

You should be all set now to access the folder/directory.

### How to Access the Shared Folder

To access the shared folder from Ubuntu/Linux system, you need your system’s IP address/hostname. To do that, open `System Settings -> Wifi -> Get the IP address`.

![IP Address Settings][6]

This step may vary if you are running different Linux distribution other than Ubuntu. You may also want to run `ip addr` to get the IP address as below.

![Finding out IP Address in Linux][7]

Once you have the address, you can open File Manager in Ubuntu/Linux systems and type below in the address bar. You should change the IP address based on your system.

You can now see that the shared folder is shown with a tiny shared icon that denotes a network share folder.

![Share Folder][8]

To access the shared folder from the **Windows system**, Open Run (Windows Key+R) or open Explorer and enter the below address. You should change the IP address and Folder name based on your system

```
\\192.168.43.19\Folder
```

You should be able to view the contents of the shared folder and modify it based on permission given.

### Wrapping Up

I have shown you how to share a folder from Ubuntu and access Windows systems via IP address. You can also follow the same steps for other Linux distributions. Do let me know in the comment box below if this article helped you.

--------------------------------------------------------------------------------

via: https://www.debugpoint.com/guide-how-share-folder-between-ubuntu-linux-windows/

作者：[Arindam][a]
选题：[lkxed][b]
译者：[译者ID](https://github.com/译者ID)
校对：[校对者ID](https://github.com/校对者ID)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://www.debugpoint.com/author/admin1/
[b]: https://github.com/lkxed
[1]: https://www.debugpoint.com/category/tutorials/
[2]: https://www.debugpoint.com/web-stories/ubuntu-22-04-review/
[3]: https://www.debugpoint.com/wp-content/uploads/2020/01/Local-Network-Share-Option.jpg
[4]: https://en.wikipedia.org/wiki/Samba_(software)
[5]: https://www.debugpoint.com/wp-content/uploads/2020/01/Folder-Sharing-Option-Install-Samba-1024x552.jpg
[6]: https://www.debugpoint.com/wp-content/uploads/2020/01/IP-Address-Settings.jpg
[7]: https://www.debugpoint.com/wp-content/uploads/2020/01/Finding-out-IP-Address-in-Linux.jpg
[8]: https://www.debugpoint.com/wp-content/uploads/2020/01/Share-Folder-1.jpg
