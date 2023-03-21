视频地址：[HTML5](https://www.bilibili.com/video/BV1x4411V75C/?spm_id_from=333.999.0.0&vd_source=f111e229e8ddffc692d57d989194e313)

---

# 1.初识HTML

> HTML：网页最基本的机构；
>
> CSS：美化网页；
>
> JavaScript：让网页动起来，产生很多交互性👉JQuery
>
> VUE：全后端分离的主流框架

---

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html5_kuangshenJava/images/1.png" alt="1" style="zoom:50%;" />

---



## 什么是HTML？

Hyper Text Markup Language（超文本==**标记语言**==）

​			超文本包括：文字、图片、音频、视频、动画等

> 网页右击👉审查元素；
>
> Chrome👉检查<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html5_kuangshenJava/images/2.png" alt="2" style="zoom:50%;" />

---



## HTML发展史

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html5_kuangshenJava/images/3.png" alt="3" style="zoom:50%;" />

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

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html5_kuangshenJava/images/4.png" alt="4" style="zoom:50%;" />

---



## HTML 基本结构

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html5_kuangshenJava/images/5.png" alt="5" style="zoom:50%;" />

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

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html5_kuangshenJava/images/6.png" alt="6" style="zoom:50%;" />

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

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html5_kuangshenJava/images/7.png" alt="7" style="zoom:67%;" />

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

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html5_kuangshenJava/images/8.png" alt="8" style="zoom:67%;" />

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

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html5_kuangshenJava/images/9.png" alt="9" style="zoom:67%;" />

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
  - 无论内容多少，**该元素独占一行**
  - p、h1-h6....
- 行内元素 / 行内标签
  - 内容撑开宽度，左右都是行内元素的**可以排在一行**
  - a、strong、em...

---



# 7.列表标签

- 什么是列表
  - 列表就是信息资源的一种展示形式。它可以使信息结构化和条理化，并以列表的样式显示出来，以便浏览者能更快捷地获得相应的信息
- 列表的分类
  - 无序列表：`<ul>、<li>`
  - 有序列表：`<ol>、<li>`
  - 定义列表：`<dl>、<dt>、<dd>`

```html
<!--有序列表
    应用范围：试卷、问答....
-->
<ol>
    <li>money</li>
    <li>sex</li>
    <li>life</li>
    <li>songs</li>
    <li>art</li>
    <li>crazy</li>
</ol>

<hr/>

<!--无序列表
    应用范围：导航栏、侧边栏....
-->
<ul>
    <li>money</li>
    <li>sex</li>
    <li>life</li>
    <li>songs</li>
    <li>art</li>
    <li>crazy</li>
</ul>
<hr/>

<!--自定义列表
    dl:标签
    dt:列表名称
    dd:列表内容
    -->
<dl>
    <dt>编程语言</dt>
    <dd>Java</dd>
    <dd>Python</dd>
    <dd>Linux</dd>
    <dd>C</dd>

    <dt>position</dt>
    <dd>Beijing</dd>
    <dd>YunCheng</dd>
    <dd>Chengdu</dd>
    <dd>Shenzhen</dd>
</dl>
```



---



# 8.表格标签

- 为什么使用表格
  - 简单通用：`<table>`
  - 结构稳定
- 基本结构
  - 单元格：`border（边框）`
  - 行、列 ：`<tr>、<td>`
  - 跨行、跨列：`colspan、rowspan`

```html
<!--表格 table
  行 tr
  列 td
  border 边框

  三行四列
-->
<table border="1px">
  <tr>
<!--    colspan 跨列-->
    <td colspan="4">1-1</td>
<!--    <td>1-2</td>-->
<!--    <td>1-3</td>-->
<!--    <td>1-4</td>-->
  </tr>

  <tr>
<!--    rowspans 跨行-->
    <td rowspan="2">2-1</td>
    <td>2-2</td>
    <td>2-3</td>
    <td>2-4</td>
  </tr>

  <tr>
    <td>3-1</td>
    <td>3-2</td>
    <td>3-3</td>
<!--    <td>3-4</td>-->
  </tr>
</table>

<hr/>

<table border="1px">
  <tr>
    <td colspan="3">学生成绩</td>
  </tr>

  <tr>
    <td rowspan="2">哈哈</td>
    <td>语文</td>
    <td>数学</td>
  </tr>

  <tr>
    <td>100</td>
    <td>100</td>
  </tr>

  <tr>
    <td rowspan="2">哈哈嗨</td>
    <td>语文</td>
    <td>数学</td>
  </tr>

  <tr>
    <td>100</td>
    <td>100</td>
  </tr>
</table>
```



---



# 9.媒体元素：视频和音频

- 视频元素
  - video
- 音频元素
  - audio

```html
<!--音频和视频-->
<!--视频 video
    src：资源路径
    controls：控制条
    autoplay：自动播放
-->
<video src="../resources/video/redi.mp4" controls autoplay width="300"></video>

<!--音频 audio
    src：资源路径
    controls：控制条
    autoplay：自动播放
-->
<audio src="../resources/audio/pass.mp3" controls autoplay></audio>
```



----



# 10.页面结构分析

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html5_kuangshenJava/images/10.png" alt="10" style="zoom:50%;" />

```html
<header>  <h2>网页头部</h2>  </header>

<section> <h2>网页主体</h2></section>

<footer>  <h2>网页脚部</h2></footer>
```

> 使用者👉观察者👉开发者

---



# 11.iframe内联框架（内嵌网页）

`<iframe>`

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html5_kuangshenJava/images/11.jpg" alt="11" style="zoom: 50%;" />



```html
<!--iframe内联框架
    src：地址（必填）
    width
    height
    name
-->
<iframe src="https://www.hao123.com" name="hello" frameborder="0" width="1000px" height="800px"></iframe>
<a href="https://www.4399.com" target="hello">点击跳转</a>

<!--bilibili网页嵌入-->
<iframe src="//player.bilibili.com/player.html?aid=675814305&bvid=BV1eU4y1c7g4&cid=427993348&page=1"
        scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true">
</iframe>
```

---



# 12-18.初识表单

### 表单语法：表单post和get提交（重点）

>  `<form>`

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html5_kuangshenJava/images/12.png" alt="12" style="zoom:50%;" />

```html
<!--表单 form
    action：表单提交的位置，可以是网站，也可以是一个请求处理地址
    method：post和get 提交方式
	    get方式提交：我们可以在url中看到我们提交的信息，不安全，但高效
    	post方式：比较安全，传输大文件  如果不加密 也可以在network中看到
-->
<form action="1.我的第一个网页.html" method="get"></form>
```

---



### 表单元素格式

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/html5_kuangshenJava/images/13.png" alt="13" style="zoom:50%;" />

> name值必填



### 文本框和单选框

文本框：（文本框、密码框）

```html
<!--    文本输入框 input type="text"
        name值必填
        value="ajuicefans"  默认初始值
        maxlength="8"       最长能写几个字符
        size="30"           文本框长度
-->
	<p>名字：<input type="text" name="username" value="ajuicefans" maxlength="8" size="30"></p>

<!--    密码框 input type="password"-->
    <p>密码：<input type="password" name="pwd"></p>
```

单选框：

```html
<!--    单选框标签
        input type="radio"
        value：单选框的值
        name：表示 组  单选框就只能选一个了
		默认选项：checked
-->
	<p>性别：
        <input type="radio" value="boy" name="sex"/>男
        <input type="radio" value="girl" name="sex"/>女
    </p>
```

---



### 按钮和多选框和下拉框

多选框

```html
<!--    多选框标签
        input type="checkbox"
		默认选项：checked
		
        name一样时是组，服务器会把其想象成数组
-->
    <p>爱好：
        <input type="checkbox" value="sleep" name="hobby">睡觉
        <input type="checkbox" value="code" name="hobby">敲代码
        <input type="checkbox" value="chat" name="hobby">聊天
        <input type="checkbox" value="music" name="hobby" checked>听音乐
    </p>
```

按钮

```html
<!--    按钮
        input type="button"     普通按钮
        input type="image"      图像按钮
        input type="submit"     提交按钮
        input type="reset"      重置按钮

		value可以改变按钮中的值,即value可以给表单按钮赋值
-->
    <p>按钮：
        <input type="button" name="btn1" value="点击变长"> <!--效果可以通过js做-->
        <!--图片按钮-->
        <input type="image" src="../resources/images/666.jpg">
    </p>

    <p>
        <input type="submit">
        <input type="reset" value="清空表单"> <!--value可以给表单按钮赋值-->
    </p>
```

下拉框

```html
<!--    下拉框，列表框
		默认选中的：selected
-->
    <p>国家：
<!--        id=""后面的学习选择区用的，这里可以不用-->
        <select name="列表名称" >
            <option value="China">中国</option>
            <option value="US">US</option>
            <option value="UK" selected>UK</option>
            <option value="India">India</option>
        </select>
    </p>
```

---

### 列表框文本域和文件域

文本域

```html
<!--    文本域 textarea
        cols="50" rows="10"
-->
    <p>反馈：
        <textarea name="textarea" cols="50" rows="10">文本内容</textarea>
    </p>
```

文件域

```html
<!--    文件域
        input type="file"
        name="files"
-->
    <p>
        <input type="file" name="filesss">
        <input type="button" value="上传文件" name="upload">
    </p>
```



---

### 搜索框滑块和简单验证

简单验证

```html
<!--    邮件验证-->
    <p>邮箱：
        <input type="email" name="email">
    </p>
<!--    URL-->
    <p>邮箱：
        <input type="url" name="url">
    </p>
<!--    数字验证-->
    <p>商品数量：
        <input type="number" name="num" max="100" min="0" step="1">
    </p>
```

滑块

```html
<!--    滑块-->
    <p>音量：
        <input type="range" name="voice" min="0" max="100" step="1">
    </p>
```

搜索框

```html
<!--    搜索框-->
    <p>搜索：
        <input type="search" name="search">
    </p>
```

---

### 表单的应用

- 隐藏域：`hidden`
- 只读：`readonly`
- 禁用：`disabled`

- 增强鼠标可用性：`label`

  ```html
  <!--增强鼠标可用性
  	label
  	可以指向一个位置
  	for="mark" 指向一个id
  -->
      <p>
          <label for="mark">你点我试试</label>
          <input type="text" id="mark">
      </p>
  ```



### 表单的初级验证（高级需要用JS自己写）

- 思考：为什么要进行表单验证？
  - 减轻服务器压力
  - 保证数据安全性

- 常用方式：

  - placeholder（提示信息，用在输入框控件）

  ```html
  <p>名字：<input type="text" name="username" value="ajuicefans" placeholder="请输入用户名"></p>
  ```

  - required**(被需要的)**（非空判断）

  ```html
  <p>名字：<input type="text" name="username" value="ajuicefans" required></p>
  ```

  - pattern（正则表达式👉可以直接百度搜索“常用正则表达式”）

  ```html
  <p>自定义邮箱：
          <input type="text" name="diyemail" pattern="^[A-Za-z0-9\u4e00-\u9fa5]+@[a-zA-Z0-9_-]+(.[a-zA-Z0-9_-]+)+$">
  </p>
  ```

---



# 19.HTML总结

- HTML的基本结构
- 网页的基本标签
  - 标题标签
  - 段落标签
  - 换行标签
  - 水平线标签
  - 注释
  - 特殊符号
- 图像标签
  - img
- 超链接
  - 锚链接
  - 功能性链接（邮箱、QQ）
- 行内元素和块元素
- 列表
  - 有序
  - 无序
  - 自定义

- 表格
  - 行、列
  - 跨行、跨列
- 媒体元素
  - 音频
  - 视频
- 网页的简单布局
  - 头部
  - 主体
  - 脚部

- 内联框架：iframe
- 表单
  - form 【get / post】
  - 文本框
  - 密码框
  - 单选框
  - 多选框
  - 按钮
  - 下拉框
  - 滑块
  - ...
- 表单应用
  - 隐藏域
  - 只读
  - 禁用
- 表单的初级验证
  - 用户提示 placeholder
  - 非空判断 required
  - 正则表达式 pattern
