## 《HTML入门笔记1》
* HTML是谁发明的
* HTML 起手应该写什么
* 常用的表章节的标签有哪些，分别是什么意思（h1~h6、section、article、main、aside 等等）
* 全局属性有哪些
* 常用的内容标签有哪些，分别是什么意思（a、strong、em、code、pre 等等）
  
##### 1.HTML是谁发明的
1990年左右HTML诞生，由Tim Berners-Lee发明，我称之为李爵士。

##### 2.HTML 起手应该写什么
首先输入"!",再按Tab键一键生成。
代码如下：
```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

##### 3.常用的表章节的标签有哪些，分别是什么意思（h1~h6、section、article、main、aside 等等）
* 标题：h1~h6
* 章节：section
* 文章：article
* 段落：p
* 头部：header
* 脚部：footer
* 主要内容：main
* 旁支内容：aside
* 划分内容：div

##### 4.全局属性有哪些
* class
* contenteditable 表示将内容变为可编辑，用户可在页面直接编辑文字。
```html
<div class="middle" contenteditable>
//表示将内容变为可编辑，用户可在页面直接编辑文字。
```
* hidden
``` html
<footer hidden>
//表示将footer内容隐藏
```
* id
  用法与class类似，如果该id元素是页面唯一的，则可以用id，不到万不得已不可以使用id。
* style
  样式标签，用来标明字体，颜色，背景颜色等等。
* tabindex
```html
<footer tabindex=1>
    //无鼠标时使用Tab键点击网页的先后顺序
<footer tabindex=2>
    //tabindex的值为负数则不可用Tab键选中，为0则排序为最后一个  
```
* title
```html
<footer title="完整的内容">
//鼠标停留在该元素上会显示“完整的内容”字样
```
##### 5.常用的内容标签有哪些，分别是什么意思（a、strong、em、code、pre 等等）
* ol+li：有序列表
* ul+li：无序列表
* dl+dt+dd：用来描述列表
```html
<dl>
    <dt>思思</dt>//被描述对象
    <dd>大美女</dd>//描述的内容
</dl>    
```
* pre：用来保留空格，回车等
```html
<pre>
    第一章：       内容
</pre>
```
* code： code中的字体是等宽的并且字体很小 
* hr：水平分割线
* br：换行
* a：打开链接
```html
<a herf="http://qq.com" target="_blank">
    //"_blank"表示在新的页面打开链接
```  
* em：表示（语气）加重，字体变为斜体
* strong：表示（本质）加重，字体变为加粗
* quote：引用（内联样式）
* blockquote：引用（外联样式）# blog-1
# blog-1
