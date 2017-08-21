后台外观的所有设置都已经有说明文字，这里还是补充几点。

### instantclick设置

详细文档请看：[instantclick 中文文档](https://www.ihewro.com/archives/515/)

#### 预加载模式选择

* 如果你得服务器配置不好，推荐选择`mousedown`或者`on-mouseover-with-a-delay`模式
* 服务器配置很好，推荐选择`mouseover`模式
* 选择`on-mouseover-with-a-delay`必须配置`延迟时间设置`，默认`70`

#### 延迟时间设置

* 只有在`on-mouseover-with-a-delay`模式下才会有效。
* 代表了鼠标悬停在链接上一定时间才会预加载，避免误点导致额外的服务器资源开销。
* 官方推荐在50——100之间的整数。

### 七牛镜像存储

![qiniu](https://ihewrocdn.b0.upaiyun.com/img/qiniui.png)

左边填写的是你的博客的附件存放的地址，右边填写的是你的七牛空间地址。

注意：你的七牛空间必须在镜像存储的设置项中填写你的博客的附件存放的地址，这样才能达到加速的效果。

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
