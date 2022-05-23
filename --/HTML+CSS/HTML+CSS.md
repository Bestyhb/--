
[TOC]

1. HTML介绍
    1.1 HTML概述
    1.2 HTML发展史
    1.3 HTML文档（网页）
        1.3.1 网页编辑工具
        1.3.2 HTML文档的基本机构
        1.3.3 HTML标签的分类
        1.3.4 HTML标签的属性
2. 集成开发工具IDE
3. 常见的HTML标签
换行标签 <br/>
标题标签 <h1>~<h6> 属性：对其方式 align ，值 center 居中 right 居右 left 居左
段落标签 <p></p>
水平线标签 <hr/> 
加粗
斜体
删除线
空格
图像标签 <img src="path" width="100px" height="10px"/>
表格标签 <table></table> 行 <tr></tr> 单元格 <td></td> 确定内容有几行几列，有几行就添加几对tr，有几列就在每行tr中添加几对td。水平方向合并单元格

段落：p
换行：br
超链接 <a href=">
a
图片：img
表格：table: colspan\rowspan
标记文本：span

------
1. CSS介绍
    1.1 什么是CSS
    1.2 CSS优势
    1.3 CSS发展历史
2. CSS样式表的引入方式
    2.1 行内（内联）样式
    2.1 内部样式表
    2.3 外部样式表
3. CSS3基本选择器
    3.1 选择器基本语法
    3.2 选择器类型
        3.2.1 标签选择器
        3.2.2 类选择器
        3.2.3 id选择器
        3.2.4 通用选择器
        3.2.5 分组选择器
4. CSS样式应用
    4.1 常见的样式属性
    4.2 CSS美化超链接

### 1.1 什么是CSS
Cascading Style Sheet，层叠样式表单，用于表述HTML文档样式的语言。
（通过CSS选择器与HTML元素相结合）有效地设置页面及页面各元素的样式，例如布局、字体、背景。
### 1.2 CSS优势
- 内容与表现分离。
- 网页表现统一，容易修改。
- 丰富的样式，使得页面布局更为灵活。
- 增加网页加载速度，节省网络带宽。

### 1.3 CSS发展历史
1996年，W3C机构制定发布了CSS1.0（第一版）。
> 该版本在99年时，经过修正，主要提供了一些简单的样式表机制，让程序员可以通过style标签或者标签上的某些属性对标签内容进行控制。
> 
1998年，W3C机构发布了CSS2.0(第二版)。
> 该版本包含1.0内容，扩展、更正、增加了更多更强的属性。CSS2.0支持多媒体样式表，让程序员通过CSS使不同设备上的网页文档显示相同的效果。
> 
2001年，CSS3.0发布。
> CSS3.0遵循模块化开发。该标准将整个网页系统划分为众多相互独立的子模块，让程序员根据不同的模块进行开发与设计对应的CSS，从而减少CSS体积。


## CSS样式的引入方式

### 2.1 行内（内联）样式
使用style属性引入css样式  
```html
<!DOCTYPE=html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>CSS的引入</title>
    </head>
    <body>
        <h1 style="color:pink">CSS</h1>
        <p>美化页面和设置各元素的显示样式</p>
    </body>
</html>
```
### 2.2 内部CSS
CSS代码写在head标签中的style标签中。  
优点：方便在同页面中修改样式。  
缺点：不利于在多页面间共享、复用、维护代码，不能够实现内容与样式代码分离。  
```html
<!DOCTYPE=html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>CSS的引入</title>
        <style type="text/css">
            h1{color:pink;}
        </style>
    </head>
    <body>
        <h1>C Style Sheet</h1>
        <p>美化页面和设置各元素的显示样式</p>
    </body>
</html>
```
### 2.3 外部CSS
1. CSS代码保存在扩展名为.css的文件中。
2. 在HTML文件中引用外部样式表。
```html
<!DOCTYPE=html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>CSS</title>
        <link href="style.css" rel="stylesheet" type="text/css"/>
    </head>
    <body>
        <h1>CSS</h1>
        <p>美化页面和设置各元素的显示样式</p>
    </body>
</html>
```

## CSS基本选择器

### 选择器基本语法
选择器名称{
属性1：属性值；
属性2：属性值；
......
}
> CSS属性最后一条的分号，可写可不写。基于W3C标准规范考虑，建议最后一条属性的结束分号（；）都要写上。
### 选择器类型
标签选择器、类选择器、id选择器、通用选择器、分组选择器
> 选择器名称不可以数字开头
选择器优先级：ID选择器>类选择器>标签选择器

#### 3.2.1 标签选择器
标签选择器：定义某类标签的样式，标签名{属性：值}  
syntax: 标签名{属性名：属性值；}
**练习：**
使用标签标题和段落标签制作任意一首古诗，并设置诗的正文字体颜色为绿色。字体大小为14px。

#### 3.2.2 类选择器
类选择器：定义某个样式类  
syntax: 类名{属性：值}
> 类名不能以数字开头命令
> 类选择器能够多次使用
```HTML
<!DOCTYPE=html>
<html>
    <head>
        <meta charset="utf-8">
        <title>CSS样式表的引入</title>
        <style tpye="text/css">
            .blue{
                color:blue;
            }
        </style>
    </head>
    <body>
        <h1>如梦令</h1>
        <p>昨夜雨疏风骤，浓睡不消残酒。</p>
        <p>试问卷帘人，却道海棠依旧。</p>
        <p class="blue">知否？知否？</p>
        <p class="blue">应是绿肥红瘦。</p>
    </body>
</html>
```

#### 3.2.3 id选择器
ID选择器：定义ID标签的样式  
syntax: ID名{属性：值}
> 一般应用于指定的元素。
> id名称不能以数字开头。

元素的id在页面中是唯一的，因此id选择器用于选择唯一的元素。
```HTML
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>CSS样式表的引入</title>
        <style type="text/css">
            #first{fontsize:20px;}
            #second{background-color:plum;}
        </style>
    </head>
    <body id="second">
        <h1>如梦令</h1>
        <p id="first">昨夜雨疏风骤，浓睡不消残酒。</p>
        <p>试问卷帘人，却道海棠依旧。</p>
        <p>知否？知否？</p>
        <p>应是绿肥红瘦。</p>
    </body>
</html>
```
**练习：**
#### 3.2.4 通用选择器
*{}中的\*代表选择html页面上的所有元素。
```CSS
*{
    text-align:center;
    color:blue;
}
```
#### 3.2.5 分组选择器
使用逗号分隔每个选择器
```CSS
h1,h2,p{
    text-align:center;
    color:red;
}
```

## CSS样式应用
### 常见的样式属性
文字字号：font-size
文字粗细：font-weight
文本水平方向对齐：text-align
> a标签通过href属性值实现页面跳转。链接页面显示在当前页面还是新页面通过target属性实现。
```
target="_self" 当前窗口打开
target="_blank" 新窗口打开

```
### CSS美化超链接
`a{text-decoration:none;}` 定义链接标签：取消链接文字下划线
`a:hover{}` 定义链接标签：鼠标放置样式
`a:active{}` 定义链接标签：鼠标点击（未释放）样式
`<a href="#"></a>` 定义链接标签：跳转自身页面，用于调试。

