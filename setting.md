后台外观的所有设置都已经有说明文字，这里还是补充几点。

### 将本地静态资源上传到你的cdn上

博客采用

### 图片附件加速

![qiniu](https://ihewrocdn.b0.upaiyun.com/img/qiniui.png)

在该项配置填写的是你的博客附件的镜像空间地址(地址以`/`结尾)。

在一般情况下，七牛镜像空间的访问文件速度要比你服务器访问文件速度要快，所以你可以建立七牛镜像空间（或者其他的镜像控件）加速你博客中的**附件访问速度**。

注意：你的七牛空间必须在`镜像存储的设置项`中填写你的**博客的附件存放的地址**(例如：https://www.ihewro.com/usr/uploads/ )，这样才能达到加速的效果。

### DNS预解析

DNS prefetching通过指定具体的URL来告知客户端未来会用到相关的资源，告诉客户端可以尽早的解析DNS。

更多详细信息，[请戳这个](https://www.linpx.com/p/small-practice-of-prefetching-dns.html)

### 首页文章摘要

 默认显示文章的前200字作为摘要，你还可以使用`摘要分隔符`进行自主截断内容输出
```markdown
<!--more-->
```

### 侧边栏的标签云

需要在新建文章的页面右侧填写标签，才会在首页侧边栏输出的。(回车添加当前标签)

![tagcloud](https://ihewrocdn.b0.upaiyun.com/img/tag.png)
