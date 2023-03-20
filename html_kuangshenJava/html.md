# 1.初识HTML

> HTML：网页最基本的机构；
>
> CSS：美化网页；
>
> JavaScript：让网页动起来，产生很多交互性👉JQuery
>
> VUE：全后端分离的主流框架

---

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html_kuangshenJava/images/1.png" alt="1" style="zoom:50%;" />

---



## 什么是HTML？

Hyper Text Markup Language（超文本==**标记语言**==）

​			超文本包括：文字、图片、音频、视频、动画等

> 网页右击👉审查元素；
>
> Chrome👉检查<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html_kuangshenJava/images/2.png" alt="2" style="zoom:50%;" />

---



## HTML发展史

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html_kuangshenJava/images/3.png" alt="3" style="zoom:50%;" />

---



## HTML5的优势

- 世界知名浏览器厂商对 HTML5 的支持
  - 微软
  - Google
  - 苹果
  - Opera
  - Mozilla
- 市场的需求
- 跨平台👉统一标准



### W3C标准

- W3C
  - World Wide Web Consortium（万维网联盟）
  - 成立于1994，Web技术领域最权威和最具影响力的**<u>国际中立性标准机构</u>**
  - http://www.w3.org/
  - http://www.chinaw3c.org/
- W3C标准包括：（面试可能会问）
  - **结构**化标准语言（HTML、XML）
  - **表现**标准语言（CSS）
  - **行为**标准（DOM、ECMAScript即JavaSctipt）



### 常见IDE（集成开发环境Integrated development Environment）

- 记事本
- Dreamweaver
- IDEA
- WebStorm

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html_kuangshenJava/images/4.png" alt="4" style="zoom:50%;" />

---



## HTML 基本结构

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html_kuangshenJava/images/5.png" alt="5" style="zoom:50%;" />

> 单个的叫 **自闭合标签**（即只用写一个）

---



# 2.网页基本信息

> 1.我的第一个网页.html

## DOCTYPE 声明

​		<!-- DOCTYPE:告诉浏览器，我们要使用什么规范 -->

​		`<!DOCTYPE html>`

- `<title>` 标签
- `<meta>` 标签

> HTML的注释如何写
>
> <!--  -->
>
> `ctrl + /`：注释快捷键
>
> 注释也会生成在HTML里，浏览器本身也是一个智能的IDE

---



## 其他标签：html、head、title、meta

`<html></html>` 标签：总的标签，网页只显示 `<html></html>` 标签内的东西

`<head></head>` 标签：代表网页头部

`<body></body>` 标签：代表网页主体

`<title></title>` 标签：代表网页标题

 `<meta>` 标签（单标签）：描述性标签，用来描述网站的一些信息（例如：`<meta charset="UTF-8">`）；一般用来做SEO（搜索引擎优化）

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html_kuangshenJava/images/6.png" alt="6" style="zoom:50%;" />

---



# 3.网页基本标签

标题标签、段落标签、换行标签、水平线标签、字体样式标签、注释和特殊符号

> 在intellij和pycharm中按 `tab` 会自动补上闭合标签

## 标题标签

```html
<h1>一级标签</h1>
<h2>二级标签</h2>
<h3>三级标签</h3>
<h4>四级标签</h4>
<h5>五级标签</h5>
<h6>六级标签</h6>
```



## 段落标签

```htm;
<p></p>
```



## 换行标签（自闭合标签）

```html
<br/>
```

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html_kuangshenJava/images/7.png" alt="7" style="zoom:67%;" />

> 换行的**间距** 比 段落标签 小



## 水平线标签（自闭合标签）

```html
<hr/>
```



## 字体样式标签

```html
<!-- 粗体 -->
<strong>哈哈</strong>

<!-- 斜体 -->
<em>哈哈</em>
```



## 注释和特殊符号

### 注释见上面

```html
<!-- 单行注释 -->

<!-- 
多行
注释
-->
```

### 特殊符号：` &    ;`

> 不知道的百度就好

#### 空格：`&nbsp;`

> 只用键盘上的空格，无论输入几个都只显示1个

#### 大于：`&gt;`

#### 小于：`&lt;`

#### 版权符号：`&copy;`

---



# 4.图像标签

常见的图像格式：JPG、GIF、PNG、BMP.......

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html_kuangshenJava/images/8.png" alt="8" style="zoom:67%;" />

```html
<!-- img 标签学习
src：图片地址（必填）
    相对地址，绝对地址

    ../ 上一级目录

alt：图片名字（必填）
    找不到的时候，会用alt替代
-->
<img src="../resources/images/666.jpg" alt="666" title="悬停文字" width="300" height="300">
```



# 5.链接标签

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html_kuangshenJava/images/9.png" alt="9" style="zoom:67%;" />

```html
<!--
    a标签
    href ： 必填，表示要跳转的那个页面
    target : 表示窗口在哪里打开
        _blank ： 在新页面打开
        _self ： 在自己的页面打开
-->

<a href="1.我的第一个网页.html" target="_blank">点击我跳转到页面一</a>
<a href="https://www.baidu.com" target="_self">点击我跳转到百度</a>

<a href="https://www.baidu.com">
<!--  图像超链接  -->
    <img src="../resources/images/666.jpg" alt="666" title="百度搜索">
</a>
```



## 超链接

- 页面间链接
  - 从一个页面链接到另一个页面
- 锚链接

```html
<!-- 使用name作为标记 -->
<a name="top">顶部</a>

<!--
    锚链接
    1. 需要一个标记  <a name="top">顶部</a>
    2. 通过 # 跳转到标记
-->
<a href="#top">回到顶部</a>
```

- 功能性链接

```html
<!--
    功能性标签
    邮件链接 ： mailto:
    qq链接 ：
-->
<a href="mailto:ajuicefans@qq.com">点击联系我</a>
```

---



# 6.行内元素和块元素

- 块元素 / 块标签
  - 无论内容多少，该元素独占一行
  - p、h1-h6....
- 行内元素 / 行内标签
  - 内容撑开宽度，左右都是行内元素的可以排在一行
  - a、strong、em...

---



# 7.列表标签

