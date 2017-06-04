#### 安装完主题后，页面错乱

A：依次检查主题文件夹名称是否为`handsome`——是否已经安装并且启用主题必要的插件


#### 点击首页头像，显示404页面

A：需要新建“时光机”独立页面，具体方法见[独立页面](/page)

#### 使用搜索功能，显示404页面

A：v3.1暂时需要开启伪静态，才能正常使用。v3.2会对此进行优化，请谅解。

#### 评论区不能斗图不能显示图片/说说不能显示图片

A：后台 `设置——评论——允许使用的HTML标签和属性` 里面添加html标签
```html
<img src="">
```

#### 评论区无法使用markdown语法

A：后台 `设置——评论——在评论中使用Markdown语法(选中)`
后台 `设置——评论——允许使用的HTML标签和属性` 里面添加html标签
```html
<blockquote><pre><code><strong><em><h5><h6><a href title><table><thead><tr><th><tbody><td>
```


#### 使用Aplayer播放器插件报错

A：这儿有解决方法：[issues #5](https://github.com/ihewro/typecho-theme-handsome/issues/5)



#### 启用主题后，无法评论

A：别着急，放轻松。点一下这个链接：[#评论系统](/comment)



#### links插件无法启用，显示500错误

A：links插件不是由我维护的，开发作者已经很久没有更新，很可能不能适用你的服务器上面（很可能没有正确的配置服务器）。如果有错误，请在typecho根目录下的`config.inc.php`里加入
```php
define('__TYPECHO_DEBUG__', true);
```
此举会输出详细的错误信息。把具体的错误信息复制，在评论区域或者发邮件给我，这样方便我更快的处理。
