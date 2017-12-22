---
layout: post
title: "antd项目在vscode中配置"
description: ""
category: tech 
tags: [react antd vscode nodejs npm 脚手架]
---

vscode 是对react是out of the box的
# 安装脚手架
```
npm install -g create-react-app
```
# 创建启动项目
```
create-react-app hu-admin 
```
这个时候项目已经启动了,如果仔细观察工程目录以及依赖，并没有发现babel以及build目录或者dist目录。往下看！
# build production
用 `create-react-app`命令创建的starter，里面会本地安装一个module：`react-script` 依赖了 babel等其他工具。这个说明可以在工程目录的README中看到。
```
npm run build
```

# server
>
The build folder is ready to be deployed.
You may serve it with a static server:
  `npm install -g serve`
  `serve -s build`

另外最近刚用vscode对terminal支持的也挺好，因为安装了git mingw，vscode竟然也很好的探测到了.:w

# 安装antd
```
npm install antd --save
``` 

最后感叹下create-react-app这个工具优秀的地方，看到.gitignore都给我写好了，自动node_modules过滤掉真是良心！

