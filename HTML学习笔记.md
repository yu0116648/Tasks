# HTML学习笔记

## 环境搭建

VS Code是一个非常好用的工具，进行前端开发需要先安装两个插件：**HTML CSS Support**、**Live Server**、**Auto Rename Tag**

使用LIve Server可以将我们编辑的内容**实时**在浏览器中显示出来，让我们在编辑过程中对自己所写的代码有一个具体可感的**回馈**，但是要想实现这一功能需要再VS Code 左上角**文件**那里打开**自动保存**，这样才能让我们的编辑在浏览器网页上**实时更新**

VS Code的便利之处在于，我们在编辑一条语句的时候，它能够预测我们将要编辑的语句体，会帮我们显示出来供我们选择，我们可以按下Tab键进行补全，非常方便，比如我们在搭建HTML编辑的框架时，只需按下“！”，即可识别出我们要写的内容，我们选中“！”并按下Tab后，即可自动补全

## 常见文本标签

<h1>一级标题标签</h1>
    <h2>一级标题标签</h2>
    <h3>三级标题标签</h3>
    <h4>四级标题标签</h4>
    <h5>五级标题标签</h5>
    <h6>六级标题标签</h6>
    <p>这是一个段落标签<b>字体加粗</b><i>斜体</i><u>下划线</u><s>删除线</s></p>
    <ul>
        <li>无序列表元素1</li>
        <li>无序列表元素2</li>
    </ul>
    <ol>
        <li>有序列表元素1</li>
    <li>有序列表元素2</li>
    </ol>
    <table border="1">
        <tr>
            <th>表头1</th>
            <th>表头2</th>
            <th>表头3</th>
        </tr>
        <tr>
            <td>元素1</td>
            <td>元素2</td>
            <td>元素3</td>
        </tr>
        <tr>
            <td>元素21</td>
            <td>元素22</td>
            <td>元素23</td>
        </tr>
        <tr>
            <td>元素31</td>
            <td>元素32</td>
            <td>元素33</td>
        </tr>
    </table>





## HTML属性

在上面的列表中<table border="1">中“border=”1“就是一个属性

在超链接时我们用到的target="_blank"也是属性的其中一种，这是超链接的四种属性之一，区别于其他三种属性是点击超链接以后，页面会自动生成一个新页面并跳转

<img src="证件照白.jpg" alt="" >在这一语句中，alt也是属性的一种，意味如果图片不能正常打开，alt后面“”中会显示提示内容。wideth是表示图片大小的一种属性



## HTML区块

div是一个块级标签，通常用于将页面划分为不同的部分，比如划分导航栏，网页内容部分等

通常用于创建块级容器，以便于组织页面结构和布局

具体操作为：<div class="nav">

<a href="#">链接1</a>

<a href="#">链接2</a>

<a href="#">链接3</a>

<a href="#">链接4</a>

<a href="#">链接5</a>

<div/>

span标签是将一小部分文本包装起来，以便于对它们使用样式、CSS或者是使用JS行为，它是行内元素，不会独占一行，只会占据它内容所需要的宽度

span标签用于内联样式化文本，给文本的一部分应用样式或者是标记

上述两个标签通常是和CSS和JS一起使用，这样就能实现更加复杂的页面布局和样式化

## HTML表单

## form表单

<form>
    <span>用户名：</span>
    <input type="text" placeholder="请输入内容"> placeholder是给用户一个提示信息，用户在输入框中输入内容以后提示信息就会消失
    <span>密码：</span>
    <input type="text" value="请输入内容"> value是规定value的值
</form>

其中还有与input配套使用的特定标签：lable,在这里与span标签作用一致

<label for="">性别</label>

<input type="radio">男

<input type="radio">女

<input type="radio">其他

radio属性是单选

checkbook属性是多选

submit属性是提交 提交位置：form后有一个action，会有一个UPL，与API有关，暂时不了解





