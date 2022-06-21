[#]: collector: (lujun9972)
[#]: translator: (Donkey-Hao)
[#]: reviewer: (wxy)
[#]: publisher: (wxy)
[#]: url: (https://linux.cn/article-14739-1.html)
[#]: subject: (10 ways Ansible is for everyone)
[#]: via: (https://opensource.com/article/21/1/ansible)
[#]: author: (James Farrell https://opensource.com/users/jamesf)

分享 10 篇 Ansible 文章
======

> 通过这些 Ansible 文章扩展你的知识和技能。

![](https://img.linux.net.cn/data/attachment/album/202206/21/111840akw4bjd13dh8ayky.jpg)

我希望能够激发刚刚接触 Ansible 的初学者的兴趣。这里有一系列总结文章，我已将其包括在内，以供你随意后续查阅。

### 适合初学者的 Ansible 

这五篇文章对于 Ansible 新手来说是一个非常好的起点。前三篇文章由 Seth Kenlon 撰写。
  
  * 如果你不了解 Ansible ，[现在可以做这 7 件事][2] 来入手。这是很好的入门指导，它收集了用于管理硬件、云、容器等的链接。
  * 在 《[编排与自动化有何区别？][3]》 这篇文章中，你会学到一些术语和技术路线，将会激发你对 Ansible 感兴趣。
  * 文章 《[如何用 Ansible 安装软件][4]》 覆盖了一些脚本概念和一些 Ansible 的好惯例，给出了一些本地或远程管理软件包的案例。
  * 在 [我编写 Ansible 剧本时学到的 3 个教训][5] 中，使自己养成 Jeff Geerling 所传授的好习惯，他是一位真正的 Ansible 资深人士。源代码控制、文档、测试、简化和优化是自动化成功的关键。
  * 《[我使用 Ansible 的第一天][6]》 介绍了记者 David Both 在解决重复性开发任务时的思考过程。这篇文章从 Ansible 的基础开始，并说明了一些简单的操作和任务。
  
### 尝试 Ansible 项目

一旦你掌握了基础和并拥有良好习惯，就可以开始一些具体主题和实例了。

  * Ken Fallon 在 《[使用 Ansible 管理你的树莓派机群][7]》 一文中介绍了一个部署和管理树莓派设备机群的示例。它介绍了受限环境中的安全和维护概念。
  * 在 《[将你的日历与 Ansible 融合以避免日程冲突][8]》一文中，Nicolas Leiva 快速介绍了如何使用前置任务和条件在自动日程安排中中强制执行隔离窗口
  * Nicolas 在 《[创建一个整合你的谷歌日历的 Ansible 模块][9]》中完成了他的日历隔离的理念。他的文章深入探讨了在 Go 中编写自定义 Ansible 模块以实现所需的日历连接。 Nicolas 介绍了构建和调用 Go 程序并将所需数据传递给 Ansible 并接收所需输出的不同方法。

### 提升你的 Ansible 技巧

Kubernetes 是近来的热门话题，以下文章提供了一些很好的示例来学习新技能。

  * 在 《[适用于 Kubernets 自动编排你的 Ansible 模块][10]》 文章中，Seth Kenlon 介绍了 Ansible Kubernetes 模块， 介绍了用于测试的基本 Minikube 环境，并提供了一些用于<ruby>荚<rt>Pod</rt></ruby> 控制的 `k8s` 模块的基本示例。
  * Jeff Geerling 在 《[使用 Ansible 的 Helm 模块构建 Kubernetes Minecraft 服务器][11]》 中解释了 Helm Chart 应用程序、Ansible 集合以及执行一个有趣的项目以在 k8s 集群中设置你自己的 Minecraft 服务器的概念。

我希望你的 Ansible 旅程已经开始，并能常从这些文章中充实自己。

--------------------------------------------------------------------------------

via: https://opensource.com/article/21/1/ansible

作者：[James Farrell][a]
选题：[lujun9972][b]
译者：[Donkey](https://github.com/Donkey-Hao)
校对：[wxy](https://github.com/wxy)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://opensource.com/users/jamesf
[b]: https://github.com/lujun9972
[1]: https://opensource.com/sites/default/files/styles/image-full-size/public/lead-images/innovation_lightbulb_gears_devops_ansible.png?itok=TSbmp3_M (gears and lightbulb to represent innovation)
[2]: https://opensource.com/article/20/9/ansible
[3]: https://opensource.com/article/20/11/orchestration-vs-automation
[4]: https://opensource.com/article/20/9/install-packages-ansible
[5]: https://opensource.com/article/20/1/ansible-playbooks-lessons
[6]: https://opensource.com/article/20/10/first-day-ansible
[7]: https://opensource.com/article/20/9/raspberry-pi-ansible
[8]: https://opensource.com/article/20/10/calendar-ansible
[9]: https://opensource.com/article/20/10/ansible-module-go
[10]: https://opensource.com/article/20/9/ansible-modules-kubernetes
[11]: https://opensource.com/article/20/10/kubernetes-minecraft-ansible
[12]: https://opensource.com/article/20/1/ansible-news-edition-six
[13]: https://opensource.com/article/20/2/ansible-news-edition-seven
[14]: https://opensource.com/article/20/3/ansible-news-edition-eight
[15]: https://opensource.com/article/20/4/ansible-news-edition-nine
[16]: https://opensource.com/article/20/5/ansible-news-edition-ten
[17]: https://opensource.com/how-submit-article
