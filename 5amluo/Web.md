# 一.编程基础
## 1.HTML
(HTML具体的内容可参考菜鸟教程，这里不多赘述，只记录HTML的大致组成和框架以及web安全中主要关注的html部分)
### 1.1HTML简介
- HTML 是用来描述网页的一种语言。

- HTML 指的是超文本标记语言:HyperText Markup Language
- HTML 不是一种编程语言，而是一种标记语言
- 标记语言是一套标记标签 (markup tag)
- HTML 使用标记标签来描述网页
- HTML 文档包含了HTML 标签及文本内容
- HTML文档也叫做 web 页面
### 1.2HTML简单结构
![一个简单实例](image.png)
### 1.3HTML CSS
CSS 是在 HTML 4 开始使用的,是为了更好的渲染HTML元素而引入的.

CSS 可以通过以下方式添加到HTML中:

- 内联样式- 在HTML元素中使用"style" 属性
- 内部样式表 -在HTML文档头部 <head> 区域使用<style> 元素 来包含CSS
- 外部引用 - 使用外部 CSS 文件
- 内联样式：
<p style="color:blue;margin-left:20px;">这是一个段落。</p>

## 2.CSS 
### 2.1 CSS简介
CSS 规则由两个主要的部分构成：选择器，以及一条或多条声明:![alt text](image-1.png)
选择器通常是您需要改变样式的 HTML 元素。
每条声明由一个属性和一个值组成。
属性（property）是您希望设置的样式属性（style attribute）。每个属性有一个值。属性和值被冒号分开。
### 2.2 CSS简单实例
CSS声明总是以分号 ; 结束，声明总以大括号 {} 括起来:
p {color:red;text-align:center;}
### 2.3 CSS选择器
CSS 选择器用于选择你想要的元素的样式的模式
**常见的 CSS 选择器**
下是一些常见的 CSS 选择器：
元素选择器（Element Selector）：通过元素名称选择 HTML 元素。

如下代码，p 选择器将选择所有 <p> 元素:

`p {
  color: blue;
}`
类选择器（Class Selector）：通过类别名称选择具有特定类别的 HTML 元素。

类选择器以 . 开头，后面跟着类别名称。

如下代码，.highlight 选择器将选择所有具有类别为 "highlight" 的元素。

`.highlight {
  background-color: yellow;
}`
ID 选择器（ID Selector）：通过元素的唯一标识符（ID）选择 HTML 元素。

ID 选择器以 # 开头，后面跟着 ID 名称。

如下代码，#runoob 选择器将选择具有 ID 为 "runoob" 的元素。

`#runoob {
  width: 200px;
}`
属性选择器（Attribute Selector）：通过元素的属性选择 HTML 元素。属性选择器可以根据属性名和属性值进行选择。

如下代码，input[type="text"] 选择器将选择所有 type 属性为 "text" 的 <input> 元素。

`input[type="text"] {
  border: 1px solid gray;
}`
后代选择器（Descendant Selector）：通过指定元素的后代关系选择 HTML 元素。

后代选择器使用空格分隔元素名称。

如下代码，div p 选择器将选择所有在 <div> 元素内的 <p> 元素。

`div p {
  font-weight: bold;
}`

## 3.JS
### 3.1JS 简介
JavaScript 是互联网上最流行的脚本语言，这门语言可用于 HTML 和 web，更可广泛用于服务器、PC、笔记本电脑、平板电脑和智能手机等设备。
### 3.2 DOM
- 通过 HTML DOM，可访问 JavaScript HTML 文档的所有元素。
HTML DOM 模型被构造为对象的树：
![alt text](image-2.png)
- 查找 HTML 元素
通常，通过 JavaScript，您需要操作 HTML 元素。

为了做到这件事情，您必须首先找到该元素。有三种方法来做这件事：

>通过 id 找到 HTML 元素
`var x=document.getElementById("intro");`
如果找到该元素，则该方法将以对象（在 x 中）的形式返回该元素。
如果未找到该元素，则 x 将包含 null。

>通过标签名找到 HTML 元素
本例查找 id="main" 的元素，然后查找 id="main" 元素中的所有 <p> 元素：
`var x=document.getElementById("main");var y=x.getElementsByTagName("p");`

>通过类名找到 HTML 元素
本例通过 getElementsByClassName 函数来查找 class="intro" 的元素：
`var x=document.getElementsByClassName("intro");`
