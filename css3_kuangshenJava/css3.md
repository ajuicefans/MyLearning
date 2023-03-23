HTML5 + CSS3 + JavaScript

结构 + 表现 + 交互

---

视频地址：[CSS3](https://www.bilibili.com/video/BV1YJ411a7dy/?spm_id_from=333.1007.top_right_bar_window_custom_collection.content.click&vd_source=f111e229e8ddffc692d57d989194e313)

---



# 1.什么是CSS？

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

![1](https://raw.githubusercontent.com/ajuicefans/mylearning/main/css3_kuangshenJava/images/1.png)

----



## 1.3 CSS快速入门

内部样式表

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>1.我的第一个css程序</title>
<!--    内部样式表
		
		规范,<style> 可以编写css的代码 每一个声明最好使用分号 ; 结尾
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

建议使用这种规范：外部样式表

<img src="https://raw.githubusercontent.com/ajuicefans/mylearning/main/css3_kuangshenJava/images/2.png" alt="2" style="zoom:50%;" />



css的优势：

1. 内容和表现分离
2. 网页结构表现统一，可以实现复用
3. 样式十分丰富
4. 建议使用独立于html的css文件
5. 利用SEO，容易被搜索引擎收录！（vue不容易被收录）



## 1.4 CSS的3种导入方式

- 行内样式
- 内部样式
- 外部样式

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>2.导入方式</title>
    
<!--内部样式-->
    <style>
        h1{
            color: green;  
        }
    </style>
    
<!--外部样式-->    
    <link rel="stylesheet" href="css/style.css">
    
</head>
<body>

<!--优先级：就近原则：谁离这个元素最近，优先级就越高-->

<!--行内样式：在标签元素中，编写一个style属性，编写样式即可
    不符合 结构 与 表现 分离
    -->
<h1 style="color:red">ajuicefans</h1>

</body>
</html>
```

> 拓展：外部样式两种写法

- 链接式：

  html

  ```html
  <!--外部样式-->    
      <link rel="stylesheet" href="css/style.css">
  ```

- 导入式（先出现架子，再一下子变得好看）

  @import 是 css2.1 特有的！

  ```html
  <!--导入式 外部样式 CSS2.0-->
      <style>
          @import url("css/style.css");
      </style>
  ```



# 2.选择器

作用：选择页面上的某一个或某一类元素

整个调试都可以在浏览器上完成，完成后把代码copy过去就好了



## 2.1 基本选择器

1. 标签选择器：选择一类标签    `标签{}`

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <title>1.标签选择器</title>
   
       <style>
           /* 标签选择器，会选择到页面上所有的这个标签的元素 */
           /* 选择这个标签，只需要这个标签的名字 */
           h1{
               color: #4c87c7;
               background: #e5bce8;
               border-radius: 24px;
           }
           p{
               font-size: 80px;
           }
       </style>
   
   </head>
   <body>
   
   <!---->
   <h1>ajuicefans</h1>
   <h1>ajuicefans</h1>
   <p>legends never die</p>
   
   </body>
   </html>
   ```

2. 类选择器 class：选择所有class属性一致的标签，可以跨标签  `.类名{}`

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <title>2.类选择器</title>
   
       <style>
         /* 类选择器的格式： .class的名称{}
             好处：可以多个标签归类，是同一个class；可复用
         */
         .ajuicefans{
           color: #e5bce8;
         }
   
         .hahaha{
           color: beige;
         }
       </style>
   
   </head>
   <body>
   
   <h1 class="ajuicefans">标题1</h1>
   <h1 class="hahaha">标题2</h1>
   <h1 class="ajuicefans">标题3</h1>
   
   <p class="ajuicefans">你看看</p>
   
   </body>
   </html>
   ```

3. id 选择器：全局唯一！  `#id名{}`

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <title>3.id 选择器</title>
   
     <style>
       /* id选择器
           格式：#id名称{}
           id 必须保证全局唯一！
        */
       #ha{
         color: red;
       }
   
       .style1{
         color: aquamarine;
       }
   
       h1{
         color: #4c87c7;
       }
     </style>
   
   </head>
   <body>
   <!--优先级：不遵循就近原则：固定的
       id选择器 ＞ 类（class）选择器 ＞ 标签选择器-->
   <h1 id="ha">标题1</h1>
   <h1 class="style1">标题2</h1>
   <h1 class="style1">标题3</h1>
   <h1>标题4</h1>
   <h1>标题5</h1>
   <h1>标题6</h1>
   
   </body>
   </html>
   ```

> 优先级：不遵循就近原则：固定的👉id选择器 ＞ 类（class）选择器 ＞ 标签选择器

---



## 2.2 层次选择器

层次选择器不改变本身样式

- body
  - p1
  - p2
  - p3
  - ul
    - li
      - p4
    - li
      - p5
    - li
      - p6

---

1. 后代选择器：在某个元素的后面   祖爷爷-爷爷-爸爸-你

   ```css
   /* 后代选择器 这里是body之后的p标签（p标签中的也一起变）全变 */
   body p{
   	background: red;
   }
   ```

2. 子选择器：一代 儿子

   ```css
   body>p{
       /* 只有body下的第一代的所有元素变 p标签中的不变 */
       background: red;
   }
   ```

3. 相邻兄弟选择器：同辈

   ```css
   /* 相邻兄弟选择器 对下不对上 只有一个 即下一个兄弟元素会变 */
   .active + p{
       background: #4c87c7;
   }
   ```

4. 通用选择器

   ```css
   /* 通用选择器 当前选中元素的向下的所有兄弟元素 对下不对上*/
   .active~p{
       background: green;
   }
   ```

> 定位一个元素，可以修改后续的元素



## 2.3 结构伪类选择器
