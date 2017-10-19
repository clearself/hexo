---
title: express 生成项目
date: 2017-10-18 09:24:10
description: "Express 是一个简洁而灵活的 node.js Web应用框架, 提供了一系列强大特性帮助你创建各种 Web 应用，和丰富的 HTTP 工具。使用 Express 可以快速地搭建一个完整功能的网站，它有一套健壮的特性，可用于开发单页、多页和混合Web应用。此文介绍如何使用Express搭建多人博客。"
tags: express
---
## 安装 express 命令行工具，使用它我们可以初始化一个 express 项目。
```bush
$ npm install -g express-generator
```
## 新建一个工程，在命令行中输入：
```bush
$ express -e blog
```
##### 这里的-e代表的事模板引擎是.ejs。默认使用的是.jade模板引擎
![描述](https://clearself.github.io/fly/markdown/image/express_1.png "图片描述")
##### 生成的项目目录
![描述](https://clearself.github.io/fly/markdown/image/express_2.png "图片描述")
##### 进入项目下载安装依赖,建议使用淘宝镜像
```bush
$ cd blog
$ npm install
```
##### 建议使用淘宝镜像下载速度快些
```bush
$ npm install -g cnpm --registry=https://registry.npm.taobao.org
```
### 启动项目有两种方式，看个人习惯进行选择
##### 1、运行启动项目：
```bush
$ npm start
```
##### 打开浏览器http://localhost:3000/ 出现下图所示说明启动成功了
![描述](https://clearself.github.io/fly/markdown/image/express_3.png "图片描述")
##### 2、运行启动项目前修改app.js在module.exports = app;前面添加一句app.listen(port); port是端口名,然后运行：
![描述](https://clearself.github.io/fly/markdown/image/express_5.png "图片描述")
```bush
$ node app
```
##### 打开浏览器http://localhost:port/ 即可

##### 将模板引擎改成html需要修改app.js,将app.set('view engine', 'ejs')改成app.set('view engine', 'html');并且添加app.engine('html',require('ejs').__express);//两个下划线如下图
##### 还需要在views文件下建一个error.html的文件否则会报错
![描述](https://clearself.github.io/fly/markdown/image/express_6.png "图片描述")
