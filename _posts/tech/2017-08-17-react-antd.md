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
安装的node是`v8.2.1`已经开始支持ES6了,也就是说不需要babel编译器了。

# server
>
The build folder is ready to be deployed.
You may serve it with a static server:
  `npm install -g serve`
  `serve -s build`


另外最近刚用vscode对terminal支持的也挺好，因为安装了git mingw，vscode竟然也很好的探测到了.:w
