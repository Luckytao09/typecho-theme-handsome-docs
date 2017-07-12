主题内置typecho原生评论系统，同样支持任何第三方评论服务（如：多说，disqus，畅言等）。

### 使用原生评论系统

 你需要关闭`设置->评论->开启反垃圾保护`和`设置->评论->检查评论来源页 URL选项`

Q：为何需要关系两个选项？
A：typecho自带的`开启反垃圾保护`是在主题的head标签内插入一段防垃圾js，主题为了兼容pjax,将该段js内置在主题的footer标签内。也就是主题已经默认开启了反垃圾保护，再次开启后台开关，会导致冲突无法评论。而且typecho自带的反垃圾保护功能非常弱，基本是鸡肋的功能。

Q：如何防止垃圾评论？
A：推荐[SmartSpam](https://handsome.ihewro.com/#/typecho)

![使用typecho原生评论][1]


[1]: https://www.ihewro.com/usr/uploads/2017/03/343938553.jpg

### 使用第三方评论系统

找到主题目录下的component/comments.php ，删掉里面所有内容，增加第三方评论系统的代码。（不推荐）
