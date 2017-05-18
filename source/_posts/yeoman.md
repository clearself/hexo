---
title: react脚手架安装yeoman
date: 2017-05-17 19:54:55
description: "但是有些项目可以使用这种方式，但有些却不太适合，或者我们就是想要去尝试新的框架。比如最近我就尝试着使用了webpack+react+es6的方式开发项目，感觉很不错，然后很多项目都用了这种方式。所以为了不需要每次开发的时候都从头开始新建文件，就想着能不能弄个工具，使用命令能够快速的生成这样一套跑的通的项目模版，正好，有个工具叫yeoman。"
tags: yeoman
---

## react脚手架安装yeoman

### 安装脚手架,首先确保自己安装了nodejs，然后全局安装yeoman

``` bash
$ npm install -g yo
```
### 然后直接安装脚手架

``` bash
$ npm install -g generator-reactpackage
```
### 创建React项目,在合适的地方新建一个文件夹，在文件夹下运行：

``` bash
$ yo reactpackage
```
### 然后就会在此目录下生成以下目录结构：

![描述](https://clearself.github.io/fly/markdown/image/react_yo.png "图片描述")

### 调试打包React项目,然后使用以下命令：

``` bash
$ npm run dev // 项目开发过程使用，启动服务，实时刷新
$ npm run build // 开发完成之后打包文件（js、css分开打包）
```


### 测试预览项目

本项目默认监听端口是8888，所以在浏览器输入 http://localhost:8888，或者index.html->右键打开方式->chrome 就能看到效果了 如果执行上述命令提示错误：Error: getaddrinfo ENOTFOUND localhost，在host文件里面添加127.0.0.1 localhost即可 监听端口和实时刷新的功能都能在webpack.config.js文件中修改配置
