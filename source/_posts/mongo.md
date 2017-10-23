---
title: mongo在window下安装配置与启动haahha
date: 2017-10-20 16:05:58
description: "MongoDB 是一个基于分布式文件存储的数据库。由 C++ 语言编写。旨在为 WEB 应用提供可扩展的高性能数据存储解决方案。是一个介于关系数据库和非关系数据库之间的产品，是非关系数据库当中功能最丰富，最像关系数据库的。"
tags: mongo
---
### mongodb的安装 window下

##### 在官网上下载zip，这个我装在D盘的mongoDB目录下
##### 1、在D盘中创建 mongoDB 文件夹然后把下载的包解压后把其中的 bin 文件夹拷贝到创建的 mongoDB 文件夹中，并且将bin文件夹所在路径配置到环境变量PATH中用;号分开
##### 2、然后在 mongoDB文件夹中创建一个 data 文件夹，再在 data 文件夹中创建 db 文件夹
##### 3、然后在 mongoDB文件夹中创建一个 log 文件夹，再在 log 文件夹中创建 mongoDB.log文件
##### 4、然后在 mongoDB文件夹中创建一个 mongodb.config文件 并配置如下图
![描述](https://clearself.github.io/image/mongo_1.png "图片描述")
##### 打开cmd命令行进入到D:\MongoDB\bin运行mongod --config D:\MongoDB\mongodb.config 启动mongo服务
![描述](https://clearself.github.io/image/mongo_2.png "图片描述")
##### 再打开-个cmd命令 运行 mongo就会出现下图所示说明你的mongo已经运行了
![描述](https://clearself.github.io/image/mongo_3.png "图片描述")
