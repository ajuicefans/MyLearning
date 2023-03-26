视频地址：[黑马程序员Linux2023](https://www.bilibili.com/video/BV1n84y1i7td/?spm_id_from=333.999.0.0&vd_source=f111e229e8ddffc692d57d989194e313)

# Linux 第二章（黑马程序员）

## 01 Linux目录结构

### Linux目录结构

![10](https://raw.githubusercontent.com/ajuicefans/mylearning/main/Linux/heima_coder/images/10.png)



### Linux路径的描述方式

- Linux：/
- Windows：\

![11](https://raw.githubusercontent.com/ajuicefans/mylearning/main/Linux/heima_coder/images/11.png)



### 总结：

1. Linux操作系统的目录结构

   Linux只有一个顶级目录，称之为：根目录

   Windows系统有多个顶级目录，即各个盘符

2. `/` 在Linux系统中表示？

   - 出现在开头 `/` 表示：根目录
   - 出现在后面 `/` 表示：层次关系



### 课后练习：

请根据语言描述，写出对应的Linux路径：

在根目录下有一个文件夹test，文件夹内有一个文件hello.txt，请描述文件的路径

>  `/test/hello.txt`

在根目录下有一个文件itheima.txt，请描述文件的路径

> `/itheima.txt`

在根目录下有一个文件夹itcast，在itcast文件夹内有文件夹itheima，在itheima文件夹内有文件hello.txt，请描述文件的路径

>  `/itcast/itheima/hello.txt` （层次关系）





## 02 Linux命令基础

### 什么是命令、命令行？

命令行效率远远大于图形化界面

学习Linux本质上就是学习在命令行中熟练使用Linux的各类命令

![12](F:\lifeProject\Mylearning\Linux\heima_coder\images\12.png)



### Linux命令基础格式

![13](F:\lifeProject\Mylearning\Linux\heima_coder\images\13.png)

示例：

- `ls -l /home/ajuicefans`：`ls` 是命令本身，`-l` 是选项，`/home/ajuicefans` 是参数
  - 意思是：以**列表的形式**，显示`/home/ajuicefans` 目录内的内容
- `cp -r test1 test2`：`cp` 是命令本身，`-r` 是选项，`test1` 和 `test2` 是参数
  - 意识是：复制文件夹 `test1`，成为 `test2`



### 总结：

1. 什么是命令、命令行？

   - 命令：即Linux操作指令，是系统内置的程序，可以**以字符化的形式发出指令，操作OS**
   - 命令行：即Linux终端，可以提供字符化的操作页面供命令执行（**提供字符化的命令反馈**）

2. 掌握Linux命令的基础格式

   `command [-options] [parameter]`

   - 命令本体，即命令本身
   - 可选选项，控制命令的行为细节
   - 可选参数，控制命令的指向目标

---





## 03 ls 命令入门

### ls 命令

ls 命令的作用是**列出目录下的内容**，语法细节如下：

**语法**：`ls [-l -h -a] [参数：Linux路径]`

- `[-l -h -a]` 是**==可选==**的选项
  - -l，以列表形式查看
  - -h，配合-l，以更加人性化的方式显示文件大小
  - -a，显示隐藏文件
- 参数：被查看的文件夹，不提供参数，表示查看当前工作目录
  - Linxu路径是此命令**==可选==**的参数



### 总结：

1. 对照图像化界面，快速体验第一个命令 `ls`
2. 理解什么是 `HOME` 目录、当前工作目录