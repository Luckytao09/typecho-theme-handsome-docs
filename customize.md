


主题外观设置中提供了非常简单的自定义设置，无需修改主题源码即可配置以下自定义栏目。

配置中可以实现两个功能，一种是 **添加自定义栏目/按钮**，另一种是**隐藏主题默认栏目/按钮**。
```
1. 左侧导航栏目

2. 顶部导航按钮

3. 时光机的社会化图标

4. 时光机的联系方式内容
```

![customize](https://ihewrocdn.b0.upaiyun.com/img/customise.png)

<p class="warn">下面配置中所有的可用网页图标列表，参考[图标列表](/icons)</p>


## 左侧边栏导航

**添加自定义按钮：**

* `name`：代表显示栏目/按钮的名称
* `class`：表示栏目/按钮的网页图标的样式
* `link`：代表栏目/按钮的链接
* `target`（可选）: 代表定在何处打开链接文档，如`_blank`:浏览器总在一个新打开、未命名的窗口中载入目标文档。`_self`:代表在当前窗口打开。不填则为：`_blank`。[更多介绍](http://www.w3school.com.cn/tags/att_a_target.asp)

```json
{"name":"音乐","class":"fa fa-music","link":"xxx.com"},
{"name":"笔记","class":"fa fa-book","link":"xxx.com"}
```

<p class="tip">每两项之间，用英文逗号(,)隔开，最后一项请勿加上逗号。</p>


** 隐藏默认栏目：**

左侧边栏目默认加载**首页**按钮。隐藏方法：

```json
{"name":"home","status":"hide"}
```

## 顶部导航栏目

**添加自定义按钮：**

与`左侧边栏导航`配置的书写规则完全相同：

```json
{"name":"音乐","class":"fa fa-music","link":"xxx.com"}
```

** 隐藏默认栏目：**
顶部导航按钮默认加载**闲言碎语**按钮。隐藏方法：

```json
{"name":"talk","status":"hide"}
```


## 时光机社会化图标

默认已经填入了配置，书写规则和上面基本类似：

* `name`：代表显示按钮的名称
* `class`：表示按钮的网页图标的样式
* `link`：代表按钮的链接
* `status`：当`status`值为`single`时，特指页面中的**绿色文字按钮**，此时无需填写`class`项。

```json
{"name":"twitter","class":"fa fa-twitter","link":"#"},
{"name":"facebook","class":"fa fa-facebook","link":"#"},
{"name":"googlepluse","class":"fa fa-google-plus","link":"#"},
{"name":"github","status":"single","link":"#"}
```

<p class="warn">简单配置，只需要修改"value"和"link"的值。高级配置，模仿上面的写法，增加或者删除相应的项目即可。</p>
<p class="tip">每两项之间，用英文逗号(,)隔开，最后一项请勿加上逗号。</p>


## 时光机联系方式

默认已经填写email、QQ、微博以及网易云音乐的配置：

* `name`：代表显示栏目的名称
* `img`：表示该联系方式的图标（图片格式）
* `link`：代表联系方式的地址

```json
{"name":"email","img":"https://ww4.sinaimg.cn/large/a15b4afegy1fg2pmtjbaej201s01s0aw","value":"ihewro@163.com","link":"#"},
{"name":"QQ","img":"https://ww4.sinaimg.cn/large/a15b4afegy1fg2pnirhr2j201s01va9u","value":"535425690","link":"#"},
{"name":"微博","img":"https://ww4.sinaimg.cn/large/a15b4afegy1fg2pofbz5fj201s01swe9","value":"@i超级男孩","link":"http://weibo.com/hewro"},
{"name":"网易云音乐","img":"https://ww4.sinaimg.cn/large/a15b4afegy1fg2pouholzj201s01s0ja","value":"@许多年以后我依然是我","link":"http://music.163.com/#/user/home?id=83271175"}
```

<p class="warn">简单配置，只需要修改"value"和"link"的值。高级配置，模仿上面的写法，增加或者删除相应的项目即可。</p>
<p class="tip">每两项之间，用英文逗号(,)隔开，最后一项请勿加上逗号。</p>
