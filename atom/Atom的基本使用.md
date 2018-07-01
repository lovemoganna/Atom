---
layout: post
title: Atom的基本使用
date: '2018-02-27 10:15'
tags:
  - Atom
categories:
  - Atom
---

## Atom常用命令:
```
项目内查找文件:ctrl+p
清除一行:ctrl+u
选中一行:ctrl+l
输入命令行:ctrl+shift+p
```
## git 的使用
```
1.添加到暂存区
2.添加提交信息
3. push到远程库

最重要的是你要保存文件(ctrl+s),在右侧的Git窗口下,将待提交的文件移到暂存区中,然后commit,最终push.

需要输入账户和密码.
```
图文展示:

![](http://upload-images.jianshu.io/upload_images/7505161-b0549b709222eb33.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

查看日志:

![](http://upload-images.jianshu.io/upload_images/7505161-d84110d6f6fc9bcd.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 支持了开发者工具

查看/开发人员/开发工具/

展示:

![开发者工具](images/2018/02/开发者工具.png)

类似于Google的F12.

## 支持图片解析

这真是一个最NB的技术,以前还需要图床解析到简书.

确实人家牛B,你截图完了以后,按快捷键,ctrl+shift+i.,输入以后,Atom会把图片自动给你解析到github.至于侵犯隐私什么的,我只是一个无名小卒,恐怕人家没工夫瞅咱把.

展示

![自动解析文件到GitHub](images/2018/02/自动解析文件到github.png)

这个图片其实是保存在本地,Atom给你解析准成链接到GitHub了.

我们可以可以随便拿出一张链接看看:
```
https://github.com/lovemoganna/Atom/blob/master/images/2018/02/%E6%B5%8B%E8%AF%95%E5%9B%BE%E7%89%87.png
```
这个用的最爽!!!

## git-plus的使用

一开始我不知道怎么用,但是探索一下就知道怎么用了.说明一个问题:别上火,慢慢来,你就会了.

就拿上面的图片上传来说.

1. 你需要进入,总命令行: `ctrl+shift+p`
2. 下面的命令都是选择带有git-plus的命令的.
2. 输入`git add all`
3. 输入`git commit all`或者不厌其烦的一个个commit.会出现一个文件,你在第一行输入commit信息,ctrl+s保存就可以commit了.
4. 输入`git push`,你要是没用github关联Atom,还要输入它的Token.就不用一遍一遍的输入用户名和密码了.

或者先用原生的命令关联远程仓库

`git remote add origin 你的GitHub仓库地址`

第一次坑爹,要合并参仓库,就是那个README.md惹的祸.

输入`git pull --rebase origin master`就可以了
