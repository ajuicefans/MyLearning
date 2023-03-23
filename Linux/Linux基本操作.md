# Linux基本操作



## pwd（旅程开始，知道你在哪里）

pwd：print working directory：**打印当前的工作目录**

```
# pwd
/
```

`/` 这是根目录，Linux里的目录像一颗倒挂的树，最顶层的目录，就是这个根目录，用一个`/`表示



## ls（旅行途中，看看你的周围都有什么）

ls：list 这个单词的缩写，即列表：**列出当前目录下的所有文件**

```
# ls
```

> 在Linux中，一切皆文件，目录在Linxu里也是一种特殊的文件



## cd（在旅途中走一走）

cd：change directory：更改目录

```
当前目录下，如果有home目录，可以直接进行如下操作
# cd home
```

```
返回上一级目录
# cd ..
```



---

# 扩展

### 无论在哪个目录下，可以直接查看根目录下的内容，且不跳转到根目录

```
# ls /
```



### 直接到达想去的目录

- 绝对路径：以系统根路径 `/` 为起点，一级一级往后面走
- 相对路径：以当前目录为起点，一级一级往要去的目录走   如果要返回上一级（`../`），要用到 `./../` （这里的`./`是指当前目录，可省略）

```
假设现在在home目录，上一层是根目录
# cd /user/bin
# cd ./../user/bin
# cd ../user/bin
```



### 清除当前的屏幕

```
# clear
```



## ls的进阶

以更加详细的方式展示内容

```
# ls -l /
# ls -l -h /
```

这里的 `l` 对应的英文单词是 `long` ，就是以长列表的形式展示信息

这里的 `h` 对应的英文单词是 `human` ，就是以人类可读的方式来展示数据

<img src="F:/lifeProject/Mylearning/Linux/images/1.png" alt="image-20230323194024101" style="zoom:67%;" />



---



# 记不住命令，怎么办？

## 查找帮助

```
# ls -h
# ls --help
# 相应指令 --help
打印出对应命令的所有用法
```

man手册

```
# man cd
# man 相应指令
按q即可退出
```





# 回顾

![image-20230323194617375](F:/lifeProject/Mylearning/Linux/images/2.png)

![image-20230323194646231](F:/lifeProject/Mylearning/Linux/images/3.png)