# sillyChooser
只会随机回答选择性问题的姬器人插件

## 使用方法
## 安装
```sh
npm install ArilyChan/sillyChooser
```

### 使用
```javascript
const sillyChooser = require("sillyChooser");
let sc = new sillyChooser({
    prefixs: ["!","！"], // 指令前缀，必须为单个字符，默认为["!","！"]
})

let reply = sc.apply(
    botId, // 姬器人Id
    userId, // qqId
    message // 指令
    );
```

### 注意
本插件默认自称是小阿日
如果需要更改称谓，请修改objects/sendMessageObject.js中的“小阿日”

### 自定义词典
本插件使用segment分词
在segmentUserDict文件夹下为自定义词典，可以自行修改
