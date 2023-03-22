HTML5 + CSS3 + JavaScript

结构 + 表现 + 交互

---



# 什么是CSS？

如何学习？

1. CSS是什么？
2. CSS怎么用？（快速入门）
3. **CSS选择器（重点+难点）**
4. 美化网页（文字，阴影，超链接，列表，渐变...）
5. 盒子模型
6. 浮动
7. 定位
8. 网页动画（特效效果）

> [菜鸟教程](https://www.runoob.com/)：[学习CSS3](https://www.runoob.com/css3/css3-tutorial.html)

---



## 1.1 什么是CSS？

CSS：Cascading Style Sheet 层叠级联样式表

CSS：表现（美化网页）

字体，颜色，边距，高度，宽度，背景图片，网页定位，网页浮动

> F12 开发人员工具

![baidu.com](https://raw.githubusercontent.com/ajuicefans/mylearning/main/css3_kuangshenJava/images/baidu.png)



## 1.2 CSS发展史

CSS1.0

CSS2.0：DIV（块）+ CSS，HTML与CSS结构分离，网页变的简单，SEO(搜索引擎优化)

CSS2.1：浮动，定位

CSS3.0：圆角边框，阴影，动画...	浏览器兼容性~



---

**练习格式：**

![image-20230322232309539](F:/lifeProject/Mylearning/css3_kuangshenJava/images/1.png)

----



## 1.3 CSS快速入门

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>1.我的第一个css程序</title>
<!--    规范,<style> 可以编写css的代码 每一个声明最好使用分号 ; 结尾
        语法：
            选择器{
                声明1;
                声明2;
                声明3;
            }
-->
    <style>
        h1{
            color:red;
        }
    </style>

</head>
<body>
<h1>我是标题</h1>

</body>
</html>
```

建议使用这种规范

![image-20230323000734360](F:/lifeProject/Mylearning/css3_kuangshenJava/images/2.png)



css的优势：

1. 内容和表现分离
2. 网页结构表现统一，可以实现复用
3. 样式十分丰富
4. 建议使用独立于html的css文件
5. 利用SEO，容易被搜索引擎收录！（vue不容易被收录）