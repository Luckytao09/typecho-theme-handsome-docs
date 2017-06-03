只需要修改主题目录下面的`js/OwO.json`文件

### 修改表情

主题内置两个栏目`颜文字`和`斗图`

直接在原有的代码上面做一些修改即可，比如图片替换，文字替换等。

### 增加新的表情栏目

```json
"新的表情栏目名称": {
    "type": "emoticon/emoji/image",
    "container": [
        {
            "icon": "OωO",
            "text": "Author: DIYgod"
        },
        {
            "icon": "OωO",
            "text": "Author: DIYgod"
        },
    ]
}
```

表情类别`type`有三种:

* emoticon: 颜文字
* emoji: emoji表情（比如😊😜😒这些图标，typecho的数据库类型默认不支持emoji编码）
* image: 图片表情

`container`下存储的是表情的具体内容：

* `icon`：表示的表情具体内容，`图片类型`就填img标签，`颜文字`就填具体的颜文字，`emoji表情`就填具体的emoji图标
* `text`:指的是鼠标悬停在表情上面显示的提示文字
