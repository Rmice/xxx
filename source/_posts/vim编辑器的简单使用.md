---
title: vim的简单使用
tags: [vim]
date: 2018-4-24 08:28:24
categories: vim
---
### vim编辑器的使用：
#### 模式切换
在命令模式下，我们可以直接按 i ,此时就会切换到编辑模式。
在编辑模式下，按 esc 就可以切换到命令模式。
#### 常用命令
下面介绍几个常用的命令，都是在命令模式下，输入 ==:+ #801400==命令使用
<!--more-->
1.q 退出编辑，如果文本内容被修改过，则会报错.
2.q! 强制退出编辑，如果文本内容被修改过，会丢弃此次的修改
3.x 退出编辑并保存。
还有一些命令可以在命令模式下直接执行，不需要在前面输入 :符号
比如dd命令会删除当前行，i命令会切换到编辑模式。也正是因为这些命令的存在，所以在需要修改文本前，一定要记得先按 i 进入编辑模式，不然命令和文本输入会搞混。

