title: 用hexo搭建个人博客
date: 2018-08-30  21:44
tags:
- hexo
categories:
- 笔记
---
# Hexo+Github搭建个人博客

### hexo: 快速、简洁且高效的博客框架

## 一、环境搭建

### 1、node环境

why？hexo时一款基于nodejs搭建起来的框架，hexo项目的运行以及后期
编译等都依赖于nodejs环境

* 环境监测

win+r 输入cmd 回车，然后输入node -v回车

如果提示能得到node版本号则表示设备具有node环境

如果提示node不是内部或者外部命令，则继续步骤

* node环境安装

* git环境搭建

node和git环境安装在上一篇博客内有写[这里](http://wxueqi.com/2018/08/28/%E9%85%8D%E7%BD%AE%E5%BC%80%E5%8F%91%E7%8E%AF%E5%A2%83/#more)

ps: 安装node切记不要选择中文路径


### 2、安装hexo脚手架

```
npm install hexo-cli -g
```

npm: 基于node的包管理器

install: 导入、安装

-g：修饰符，表示全局安装的意思(global)

## 二、项目搭建

### 1、初始化(新建)博客项目

* ①、在需要保存项目的位置右键git bash here
* ②、在命令行内: hexo init 项目名称 回车
* ③、进入项目目录: cd 项目名称 	
* ④、安装项目依赖包: npm install
* ⑤、启动项目服务: hexo s
* ⑥、预览项目

  浏览器地址栏输入:
                 [http://localhost:4000]()
  或  [http://127.0.0.1:4000]()
                 
### 2、项目目录介绍

```
|--_config.yml   当前项目的主配置文件，包含项目的大部分参数
|--package.json  项目配置文件，包含该依赖包的列表和版本等信息 
|--scaffolds     模板文件夹
|--source        项目的源文件
|  |--_drafts    草稿文件
|  |--_posts     发表的博客文件
|--themes        项目主题文件夹
|--.gitignore    git忽略上传的配置清单
|--node_modules  项目依赖包
|--public        编译过后的项目文件
```

###补充

* 停止服务：在启动服务所在的命令行窗口ctrl+c

* ps：如果想要访问项目，则必须启动服务





