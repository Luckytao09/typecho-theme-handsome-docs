### 博文头图

指的是**首页**、**文章页面**每篇文章顶部的图片，后台可以设置显示头图的方式。默认显示的顺序是：thumb（自定义字段）--> 第一个图片附件--> 文章第一张图片 --> 随机图片

thumb自定义字段在每篇文章底下填写。名称填：`thumb`，值
* 填图片地址：显示当前图片地址的图片
* 填`no`：则在首页和文章页面同时不显示当前文章的头图


### 文章目录树

文章中的目录树已经内置代码，**仅当文章有h2 h3 h4标题** 才会生成目录树，并且手机端不显示目录树。

**注意**：如果文章中没有`h2`标题，只有`h3 h4`标题是不会生成目录树的。

### 评论表情功能

表情图片存放在主题目录的Img/emoticon 文件夹下。默认12张图片。如果需要更改，则需要同步更改js/OwO.json `斗图`栏目的图片地址。
表情的颜文字和斗图的图片都是以json格式存储并调用的，所以修改需要对json有简单的了解即可。

### 短代码高亮文本

** \* 2.1.0及以上版本新增功能**

<div class="share">这是灰色的短代码框，常用来引用资料什么的，调用代码为 <strong>&lt;div class="share"&gt;输入文字&lt;/div&gt;</strong><br><br></div>

<div class="yellow">这是黄色的短代码框，常用来做提示，引起读者注意。调用代码为 <strong>&lt;div class="yellow"&gt;输入文字&lt;/div&gt;</strong><br><br></div>

<div class="red">这是红色的短代码框，用于严重警告什么的。调用代码为 <strong>&lt;div class="red"&gt;输入文字&lt;/div&gt;</strong><br><br></div>

<div class="lblue">这是浅蓝色的短代码框，用于显示一些信息。调用代码为 <strong>&lt;div class="lblue"&gt;输入文字&lt;/div&gt;</strong><br><br></div>

<div class="green">这是绿色的短代码框，显示一些推荐信息。调用代码为 <strong>&lt;div class="green"&gt;输入文字&lt;/div&gt;</strong><br><br></div>
