## 《HTML常用标签》
* a 标签的用法
* img 标签的用法
* table 标签的用法
* 其他感想

##### 1.a 标签的用法

直接执行js时使用：
```html
<a href="javascript:alert(1);">伪协议</a>
//为了直接执行js时使用"javascript:alert(1);"
```


想要一个a标签但是想让链接没反应，应使用"javascript:;"：
```html
<a href="javascript:;">查看</a>
```

href+id+# 跳转到指定标签：
```html
<p id="XXX">
<a href="#XXX">查看</a>
//直接跳转到名为XXX的页面
```


点击链接自动弹出发邮件选项：
```html
<a href="mailto:945552962@qq.com">发邮件</a>
```

点击链接自动弹出打电话选项：
```html
<a href="tel:18643731711">打电话</a>
```
##### 2.img 标签的用法
tips:永远不要让图片变形。
属性：alt/height/width/src
作用：发出get请求，展示一张图片。
```html
<img src="dog.png" alt="一只狗"/>
//alt="一只狗"是图片加载失败时用来提示
```
事件： onload/onerror用来提升用户使用优化，用法:
```html
<img id="XXX" width="400" src="dog.png" alt="一只狗"/>
<script>
    XXX.onload=function(){
        console.log("图片加载成功");
    }
    XXX.onerror=function(){
        console.log("图片加载失败");
        XXX.src="404.png";
    }
</script>

```
图片在手机浏览器显示时的设置：
```html
<style>
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    img{
        max-width: 100%;
        <!--设置这句最重要  -->
    }
</style>

```
##### 3.table 标签的用法
作用：制表
```html
<table>
    <thead>
        <tr>
            <th>英语</th>
            <th>数学</th>
            <th>语文</th>
        </tr>
    </thead>
    <!-- thead头部，th为字体加粗，td不加粗 -->
    <tbody>
        <tr>
            <td>90</td>
            <td>88</td>
            <td>79</td>
        </tr>
    </tbody>
    <!-- tbody内容 -->
    <tfoot>
        <tr>
            <td>空</td>
            <td>空</td>
            <td>空</td>
        </tr>
    </tfoot>
    <!-- tfoot脚部 -->
</table>
```
table的样式：
``` html
<style>
    table-layout:auto; 
    <!-- 根据表头宽度自动调整表格宽度 -->
    td,th{
        border:1px solid blue;
    }
    <!-- 将表格设置成1px的蓝色边框 -->
    border-spacing:20px;
    <!-- 设置表格间的空隙为20px -->
    border-collapse:collapse;
    <!-- 合并表格的空隙 -->
</style>
```

##### 4.其他感想
每次编写博客虽然耗时很长，就当做复习也是一种提高。
