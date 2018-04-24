---
title: Everblog印象笔记写GithubPage的博客
date: 2018-4-24
tags: [Github,hexo]
categories: hexo
---
### 先决条件
[使用GithubPage搭建自己的博客](http://fanzhenyu.me/categories/Hexo/)

### 需要解决的问题
这时大部分人选择的都是一款工具来写MarkDown。
<!--more-->
当然，即使是最简单的文本编辑器也是可以支持Md的编辑的。

但是，对于一个印象笔记的重度用户，
==如果一个笔记本组对应你的博客；
一篇笔记对应你的一篇博文。==

这样就可以写完一篇笔记后同步到你的博客上。岂不是美滋滋？

### 操作方式
使用 Hexo 主题完整步骤如下：

``` stylus
$ npm i hexo-cli -g # 全局安装 hexo-cli
$ hexo init myblog # 初始化一个 hexo 项目
$ cd myblog && npm i # 安装依赖
$ npm i everblog -g # 全局安装 everblog
$ npm i everblog-adaptor-hexo --save # 在当前 hexo 项目下安装 adaptor
$ echo "module.exports = require('everblog-adaptor-hexo')" > index.js # 在当前 hexo 项目下创建 index.js，引入 adaptor
$ DEBUG=* everblog build # 使用 everblog 构建 hexo 所需文件
$ hexo server # 启动 hexo
$ open http://localhost:4000/ # 浏览器打开博客主页
```


### 链接
时间先后顺序：
[貌似是开发者本人写的](https://zhuanlan.zhihu.com/p/32456254)；
[基于上者的另一种方式](https://zhougy0717.github.io/2017/07/03/%E5%9C%A8GitHub%E4%B8%8A%E7%94%A8Evernote+Hexo%E6%90%AD%E5%BB%BA%E4%B8%AA%E4%BA%BA%E9%9D%99%E6%80%81%E5%8D%9A%E5%AE%A2/)；
[基于前两者写的](https://itgoyo.github.io/8888/08/08/%E5%8D%B0%E8%B1%A1%E7%AC%94%E8%AE%B0-hexo%E6%90%AD%E5%BB%BA%E8%87%AA%E5%B7%B1%E7%9A%84%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2/).







### 补充
[印象笔记获取token](https://app.yinxiang.com/api/DeveloperToken.action)