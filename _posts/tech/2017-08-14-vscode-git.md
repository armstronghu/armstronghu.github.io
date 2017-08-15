---
layout: post
title: "git使用（一）"
description: "git使用学习记录"
category: 技术 代码管理
tags: [git,vscode,ssh]
---

git在15年用过一段时间，后面要找个时间系统的学习下，包括git的原理。今天记录下git在配置中一些常见的操作和需求，只和git本身配置有关。

## git 在vscode中是in-the-box
我们经常看到这样的一个软件术语：out-of-the-box 即开箱即用。而git在vscode中是in-the-box，应该是内置支持git，但需要配置。

## git 免密码提交
git有两种协议，https和ssh。在ssh下免登陆主要几个步骤：
* 生成私钥和公钥
* 在github个人站点登陆状态下，设置生成的公钥(此时已经可以在客户端提交，但是需要每次登陆和密码)
* 免密码提交关键：将ssh-agent 开启，并将ssh私钥加入到ssh-agent中


### 引用
[git配置](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)