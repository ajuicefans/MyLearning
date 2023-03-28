视频地址：[黑马程序员Linux2023](https://www.bilibili.com/video/BV1n84y1i7td/?spm_id_from=333.999.0.0&vd_source=f111e229e8ddffc692d57d989194e313)

# Linux 第一章（黑马程序员）

---

## 00 Linux导学

### why Linux？

个人桌面操作系统

- Windows
- MacOS

服务器操作系统

- Linux👉没有牛的过linux的



无论开发什么，最终都需要运行在Linux操作系统之上

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/Linux/heima_coder/images/1.png" alt="1" style="zoom:67%;" />



### 课程设计

![2](https://raw.githubusercontent.com/ajuicefans/mylearning/main/Linux/heima_coder/images/2.png)



### 如何学习Linux？

实操性强，Linux没有高深的理论知识，纯操作👉**==敲！==**就够了

---



## 01 操作系统概述

学习目标：

1. 了解操作系统的作用
2. 了解常见的操作系统



### 硬件和软件

硬件（看得见摸得到的）：计算机系统中由电子，机械和光电元件等组成的各种物理装置的总称

软件：是用户和计算机硬件之间的接口和桥梁，用户通过软件与计算机进行交流

> 而操作系统，就是软件的一类



一个完整的计算机：由硬件和OS组合而来



### 操作系统

操作系统是计算机软件的一种，它主要负责：作为**==用户和计算机硬件之间的桥梁==**，**==调度和管理计算机硬件进行工作==**

而计算机，如果没有操作系统，就是一堆无法使用的塑料而已。

---

计算机有了OS，就有了灵魂，OS可以：

- 调度CPU
- 调度内存
- 调度硬盘进行数据存储
- 调度网卡进行网络通讯
- 调度音响发出声音
- 调度打印机打印内容
- ......

![3](https://raw.githubusercontent.com/ajuicefans/mylearning/main/Linux/heima_coder/images/3.png)



### 常见的操作系统

PC端

- Windows
- Linux
- macOS

移动端：

- andriodOS
- iOS
- HarmonyOS



### 总结：

1. 计算机由哪两个主要部分组成？
2. OS是什么？有什么作用？👉软件的一类，**协助用户调度硬件工作**，充当用户和计算机硬件之间的桥梁
3. 常见的OS有哪些？

---



## 02 初识Linux

### Linux的诞生

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/Linux/heima_coder/images/4.png" alt="4" style="zoom:67%;" />



### Linux内核

内核不是给我们“普通人”使用的~

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/Linux/heima_coder/images/5.png" alt="5" style="zoom:67%;" />

---

### 下载内核源码

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/Linux/heima_coder/images/6.png" alt="6" style="zoom:67%;" />

### Linux发行版

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/Linux/heima_coder/images/7.png" alt="7" style="zoom:67%;" />

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/Linux/heima_coder/images/8.png" alt="8" style="zoom:67%;" />

### 总结：

1. Linux的诞生

   Linux由**林纳斯 托瓦兹**在**1991**年创立并发展至今成为服务器操作系统领域的核心系统

2. 什么是Linux系统的内核？

   内核提供了Linux系统的主要功能，如**==硬件调度管理的能力==**。Linux内核是免费开源的，任何人都可以查看内核的源代码，甚至是贡献源代码

3. 什么是Linux系统发行版？

   **内核无法被用户直接使用**，需要**配合应用程序**才能被用户使用。**在内核之上，封装**系统级应用程序，组合在一起就称之为**Linux发行版**

---



## 03 虚拟机介绍

学习Linux系统，就需要有一个可用的Linux系统。

如何获得？将自己的电脑重装系统为Linux？

NoNo。这不现实，因为Linux系统并不适合日常办公使用。

我们需要借助 **虚拟机** 来获得可用的Linux系统环境进行学习



### 什么是虚拟机？

借助**==虚拟化技术==**，我们可以在系统中，**==通过软件：模拟计算机硬件，并给虚拟硬件安装真实的操作系统==**。这样，就可以在电脑中，虚拟出一个完整的电脑，以供我们学习Linux系统

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/Linux/heima_coder/images/9.png" alt="9" style="zoom:50%;" />



### 总结：

1. 什么是虚拟机？

   通过**虚拟化技术**，在电脑内，**虚拟出计算机硬件，并给虚拟的硬件安装操作系统**，即可得到一台虚拟的电脑，称之为虚拟机

2. 为什么要使用虚拟机？

   学习Linux系统，**需要有Linux系统环境**。我们不能给自己电脑重装系统为Linux，所以通过虚拟机的形式，得到可以用的Linux系统环境，**供后续学习使用**。

---



## 04 安装VMware Workstation虚拟化软件

### 虚拟化软件

通过虚拟化技术，可以虚拟出计算机的硬件，那么如何虚拟呢？

我们可以通过提供虚拟化的软件来获得虚拟机。

![10](https://raw.githubusercontent.com/ajuicefans/mylearning/main/Linux/heima_coder/images/14.png)



### VMware Workstation

课程选用VMware WorkStation软件来提供虚拟机。

下载地址： https://www.vmware.com/cn/products/workstation-pro.html



### VMware Workstation安装流程

详细视频：https://www.bilibili.com/video/BV1n84y1i7td?p=5&vd_source=f111e229e8ddffc692d57d989194e313

---



### 检查虚拟网卡有没有安装成功 / 验证网络适配器是否正常

![15](https://raw.githubusercontent.com/ajuicefans/mylearning/main/Linux/heima_coder/images/15.png)

确保 **vmnet1** 和 **vmnet8** 存在：如果不存在说明安装出问题了，卸载软件，重启电脑，重新安装

![16](https://raw.githubusercontent.com/ajuicefans/mylearning/main/Linux/heima_coder/images/16.png)

---

也可以直接 `win + R` ，然后输入 `ncpa.cpl` 即可打开网络适配器选项 / 网络连接

---



## 05 VMware Workstation中安装CentOS7 Linux操作系统

### 下载CentOS操作系统

CentOS7.6

- https://vault.centos.org/7.6.1810/isos/x86_64/   (最后的/不要漏掉）

  ![17](https://raw.githubusercontent.com/ajuicefans/mylearning/main/Linux/heima_coder/images/17)

- 或者直接使用如下链接下载：https://vault.centos.org/7.6.1810/isos/x86_64/CentOS-7-x86_64-DVD-1810.iso

### 在VMware中安装CentOS操作系统

视频地址：https://www.bilibili.com/video/BV1n84y1i7td?p=6&vd_source=f111e229e8ddffc692d57d989194e313

---



## 06 MacOS安装VMware Fusion并安装虚拟机

视频地址：https://www.bilibili.com/video/BV1n84y1i7td?p=7&vd_source=f111e229e8ddffc692d57d989194e313

---



## 07 远程连接Linux系统

### 图形化、命令行

对于操作系统的使用，有2种使用形式：

- 图形化页面使用操作系统
- 以命令的形式使用操作系统

不论是Windows还是Linux亦或是MacOS系统，都是支持这两种使用形式。

- 图形化：使用操作系统提供的**图形化页面**，以**获得图形化反馈**的形式去使用操作系统。
- 命令行：使用操作系统提供的各类**命令**，以获得**字符反馈**的形式去使用操作系统。



### 使用命令行学习Linux系统

尽管图形化是大多数人使用计算机的第一选择，但是在Linux操作系统上，这个选择被反转了。

无论是企业开发亦或是个人开发，使用Linux操作系统，多数都是使用的：命令行。

---

这是因为：

Linux从诞生至今，在图形化页面的优化上，并未重点发力。所以Linux操作系统的图形化页面：不好用、不稳定。

**在开发中，使用命令行形式，效率更高，更加直观，并且资源占用低，程序运行更稳定**。

---

所以，后续的课程学习中，我们：

除了在少数需要做对照讲解的情况下会使用图形化页面

其余都会以命令行的形式去讲解Linux操作系统的使用



### FinalShell

既然决定使用命令行去学习Linux操作系统，那么就必须丰富一下工具的使用。

我们使用VMware可以得到Linux虚拟机，但是在VMware中操作Linux的命令行页面不太方便，主要是：

- 内容的复制、粘贴跨越VMware不方便
- 文件的上传、下载跨越VMware不方便
- 也就是和Linux系统的各类交互，跨越VMware不方便

**我们可以通过第三方软件，FinalShell，远程连接到Linux操作系统之上。**

并通过FinalShell去操作Linux系统。

这样各类操作都会十分的方便。

---

FinalShell的下载地址为：

Windows: http://www.hostbuf.com/downloads/finalshell_install.exe

Mac: http://www.hostbuf.com/downloads/finalshell_install.pkg

下载完成后双击打开安装。

---

具体看视频：[远程连接Linux系统](https://www.bilibili.com/video/BV1n84y1i7td/?p=8&spm_id_from=333.1007.top_right_bar_window_history.content.click)

- `ifconfig` 获得ip地址
- 在final shell中匹配ip地址即可

###  总结

1. 什么是图形化操作，什么是命令行操作？
   - 图形化操作是指使用操作系统附带的图形化页面，以图形化的窗口形式获得操作反馈，从而对操作系统进行操作、使用
   - 命令行操作是指使用各种命令，以文字字符的形式获得操作反馈，从而对操作系统进行操作、使用
2. 为什么Linux操作系统要选择命令行形式呢？
   - Linux操作系统的图形化页面不好用且不稳定
   - 使用命令行的形式操作更加高效且稳定资源占用低
   - 企业和开发者都选择命令行，所以我们也学习命令行

3. 为什么使用FinalShell连接Linux去使用
   - 操作Linux系统中间跨越VMware窗口会导致交互不太方便
   - 我们只需要使用命令行无需使用图形化，所以通过命令行远程连接使用即可
4. 如何查看Linux的IP地址并远程连接呢
   - 在Linux操作系统中，桌面空白右键点击：open in terminal
   - 输入ifconfig，即可看到IP地址
   - 在FinalShell中配置好IP地址，账号密码后即可连接成功



## 08 扩展-Win10配置WSL（ubantu）环境





## 09 扩展-虚拟机快照

