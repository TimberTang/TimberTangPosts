---
title: hexo边搭边记
date: 2017-03-07 17:34:51
tags:
---
> 读者可以去[hexo官网](https://hexo.io/)查看详细的搭建步骤 

### 必备环境
- Git
- Node.js 
	- 直接下载安装包[安装Node.js](https://nodejs.org/zh-cn/download/)
- hexo
	打开终端执行 `npm install -g hexo-cli`

### 搭建本地hexo
Hexo 只是帮你搭建本地静态博客, 如果你想让别人看到.就必须上传到github上,以下是搭建本地hexo的步奏

-  首先在你本地创建一个文件夹.目的是存放整个blog工程
-  打开终端, cd 到blog 所在的文件夹里
-  输入 `hexo init`进行初始化
-  输入 `npm install` 进行安装, 骚等片刻等待安装成功
-  输入 `npm install hexo-deployer-git --save`安装插件
-  输入 `hexo server`运行hexo 然后在浏览器中运行`http://localhost:4000`进行预览
-  本地搭建完毕,按`control + c` 停止服务, 接下来将本地环境上传到github上去

### 将本地页面发布到github上

 