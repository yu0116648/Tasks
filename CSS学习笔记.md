# CSS学习笔记

## CSS导入方式：

* 内联样式表：在head中使用style标签

  * <style>
        color:blue;
        font-size:26px;
    </style>
    
    

* 内部样式表：在标签内部使用style属性

  * <h1 style="color:red;">这是一个一级标签，使用内部样表</h1>

    

  

* 外部样式表：创建一个css文件，在css文件中编辑，需要在head中使用link标签：

* 三种导入方式优先级：内联样式> 内部样式表 >外部样式表

  

  

## CSS选择器

ID>类>标签名

### 元素选择器 

选择某一个元素进行调整美化例如：

<h2 style= "color:aqua;">这是一个二级标题</h2>



### 类选择器

给元素设置类，然后对所设置的类进行调整美化：

需要首先在head中设置style，然后在style中使用：

.highlight{

background-color: yellow}

<h3 class="highlight">这是一个类选择器示例</h3>



### ID选择器 

在head中设置style，然后在style中编辑：

#header{

font-size: 80px}

<h4 id="header">这是一个ID选择器示例</h4>



### 通用选择器

直接在head中设置style，然后在style中编辑：

*{

font-family: 'KaiTi'}

### 子元素选择器

在head中设置style，然后在style中编辑：

.father>.son{

color:yellowgreen

}

<div class="father">
    <p class="son">
        这是一个子元素选择器示例
    </p>
</div>



### 后代选择器（包含选择器）

首先在head中设置style，然后在style中编辑：

.father p{

color: brown;

font-size: larger}

<div class="father">
    <p class="son">
        这是一个子元素选择器示例
    </p>
    <div>
        <p class="grandson">
            这是一个后代选择器示例
        </p>
    </div>
</div>

子代选择器和后代选择器的区别是：

后代选择器包含子代选择器，但子代选择器不包含后代选择器

我们在使用后代选择器进行美化的时候，使用的操作会作用于子代，但是在使用子代选择器进行美化时，使用的操作不能作用于后代



### 并集选择器（兄弟选择器）

在head中设置style，然后在style中编辑：

h3+p{

background-color:red

}

然后在body中：

<p>这是一个普通的p标签</p>

<h3>这是一个兄弟选择器（并集选择器）示例</h3>

<p>这是另一个p标签</p>

这样以后的效果是在style中进行的美化操作只会作用于在h3标签下紧跟着的p标签，在h3标签上方的p标签不会受影响

### 伪类选择器

伪类选择器以“：”开头，通常是给用户交互文档结构或者其他条件下的元素应用样式

示例：

使用ID选择器：

在head中设置style，然后在style中编辑：

#element:hover{ # 当鼠标选停在上面时，文字会发生颜色变化

background-color:aqua}

然后在body中编辑：

<h3 id="element">这是一个伪类选择器示例</h3>

## 盒子模型相关属性

* 内容（content）：盒子包含的实际内容，比如文本、图片等
* 内边距（Padding）：围绕在内容的内部，是内容与边框之间的空间，可以使用‘padding属性’来设置
* 边框（Border):围绕在内容的内部，是盒子的边界，可以使用border属性来设置
  * 设置边框的优先顺序：上右下左（顺时针），如果给了三个参数，那代表没有给左边框的值，会找它对应的右边框，和右边框的值保持一致
* 外边距（Margin）：围绕在边框的外部，是盒子与其他元素之间的空间，可以使用‘margin’属性来设置

## 传统网页布局方式

* 标准流（普通流、文档流）：网页按照元素的书写顺序依次排列

  * 是由块级元素和行内元素按照默认规定的方式来排列，块级就是占一行，行内元素一行放好多个元素。

* 浮动

  * 属性用于创建浮动框，将其移动到一边，知道左边缘或右边缘触及包含块或另一个浮动框的边缘，这样即可使得元素进行浮动

  * 语法：选择器{

    float: left/right/none;

    }

  * 浮动是相对于父元素浮动，只会在父元素内部移动

  * 三大特性：

    * 脱标：脱离标准流
    * 一行显示，顶部对齐
    * 具备行内块元素特性

  * 如果父元素没有设置高度，会出现塌陷问题，消除浮动影响的两种方法：

    * 在父元素的style中设置：overflow：hidden；

      或者是使用伪元素选择器：

      

* 定位
* ‘Flexbox’和Grid‘（自适应布局）





