### 哪些栏目可以自定义

* 左侧导航栏目
* 顶部导航按钮
* 时光机的社会化图标
* 时光机的联系方式内容

修改/添加这些栏目 无需修改主题源码，也不推荐修改主题源码（不利于升级），直接通过后台的外观设置简单配置。

![customize](https://cdn.ihewro.com/img/customise.png)

配置中可以实现两个功能：
* 添加自定义栏目/按钮
* 隐藏主题默认栏目/按钮

### 添加自定义栏目/按钮

如 左侧边栏添加音乐栏目，就在左侧边栏那配置那里填写
```json
{"name":"音乐","class":"fa fa-music","link":"xxx.com"}
```
1. `name`：代表显示栏目/按钮的名称
2. `class`：表示栏目/按钮的网页图标的样式
3. `link`：代表栏目/按钮的链接

添加顶部按钮是同样的。

每两项之间，用**英文逗号(,)**隔开，**最后一项请勿加上逗号**。



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
  即
```json
{"name":"talk","status":"hide"}
```

### 时光机页面的两个配置项

默认两个配置项中已经填好了内容：

> 时光机社交按钮配置

```json
{"name":"twitter","class":"fa fa-twitter","link":"#"},
{"name":"facebook","class":"fa fa-facebook","link":"#"},
{"name":"googlepluse","class":"fa fa-google-plus","link":"#"},
{"name":"github","status":"single","link":"#"}
```

【注释】：`status`：为`single`时特指绿色按钮，不填则指上面并排的小按钮。

> 时光机联系方式配置

```json
{"name":"email","img":"https://ww4.sinaimg.cn/large/a15b4afegy1fg2pmtjbaej201s01s0aw","value":"你的邮箱地址","link":"#"},
{"name":"QQ","img":"https://ww4.sinaimg.cn/large/a15b4afegy1fg2pnirhr2j201s01va9u","value":"你的QQ号","link":"#"},
{"name":"微博","img":"https://ww4.sinaimg.cn/large/a15b4afegy1fg2pofbz5fj201s01swe9","value":"你微博账号","link":"#"},
{"name":"网易云音乐","img":"https://ww4.sinaimg.cn/large/a15b4afegy1fg2pouholzj201s01s0ja","value":"你的网易云账号","link":"#"}
```


简单配置，只需要修改`"value"`和`"link"`的值

高级配置，模仿上面的写法，增加或者删除相应的项目即可

【注意】：最后一项时，末尾不需要加逗号，否则报错。
