主题的左侧导航栏目和顶部按钮均可以通过后台的外观设置简单配置。

![customize](https://cdn.ihewro.com/img/customise.png)

配置中可以实现两个功能：
* 添加自定义栏目/按钮
* 隐藏主题默认栏目/按钮

### 添加自定义栏目/按钮

如 左侧边栏添加音乐栏目，就在左侧边栏那配置那里填写
```json
{"name":"音乐","class":"fa fa-music","link":"xxx.com"},
```
1. `name`：代表显示栏目/按钮的名称
2. `class`：表示栏目/按钮的网页图标的样式
3. `link`：代表栏目/按钮的链接

添加顶部按钮是同样的。

### 隐藏主题默认栏目/按钮

如隐藏主题默认栏目/图标

> 左侧边栏

默认栏目`首页`，对应的`name`是`home`，即
```json
{"name":"home","status":"hide"}
```

> 顶部按钮

默认按钮有两个：
* `闲言碎语`，对应的`name`是`talk`
* `日间夜间模式切换`，对应的`name`是`mode`
即
```json
{"name":"talk","status":"hide"},
{"name":"mode","status":"hide"}
```
