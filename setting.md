所有设置都已经有说明文字，这里还是补充几点。

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