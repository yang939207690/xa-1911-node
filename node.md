## node 

我们在写一个js文件后比如创建一个01.helloworld.js在用node编译时
```
console.log("hello world");
````

node 01.helloworld.js

我们还可以这样运行npm init  或者  npm init -y 



这时候会自动生成一个打包文件package.json  提供了一个执行文件

package.json
```
{
  "name": "myfile",
  "version": "1.0.0",
  "description": "失败说明",
  "main": "webpack entry----",
  "scripts": {
    "test": "node 01.helloworld.js"
  },
  "keywords": [
    "node",
    "01"
  ],
  "author": "yj",
  "license": "MIT"
}

```

其中 name 文件名 

version 版本号

"description": "失败说明",

"main": "webpack entry----",  webpack打包设置入口

"author": "yj", 作者

MIT  开发协议

## 使用gitHub把文件发送到你的服务上

1. 首先第一步要确定你是否安装了gitHub
2. 如果没安装则

https://git-for-windows.github.io下载msysgit按默认选项安装即可


3. 登陆你的gitHub 创建一个新的库底下会生成一份操作说明

其实这样你就可以按照操作说明发送文件了
```
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/yang939207690/xa-1911-node.git
git push -u origin master
```



4. 在发送的时候需要注意在你发送的文件中如果有不需要发送的文件需要创建一个.gitgnore 文件 来配置你不需要上传的文件



