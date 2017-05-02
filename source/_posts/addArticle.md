---
title: 提交文章方法
date: 2017-05-01 13:46:53
tags: [杂]
photos: [http://oj7lzlt0w.bkt.clouddn.com/haida2.jpg]
---

## 第一步

目前只允许在organzation的人员添加文章。

```bash
git clone git@github.com:shouDeveloper/blog.git
git pull
```

首先先把博客源码clone到本地。
每次添加文章之前记得先pull下。

<!--more-->

## 第二步

```bash
git checkout -b you_own-branch
```

创建自己独立的分支名。
若已经创建则记得从master分支更新下。

```bash
git merge master
```

## 第三步
创建文章

```bash
hexo new new_article_title
```

不会使用hexo的可以看下hexo语法

## 第四步

推送自己的分支到远程仓库，然后给我提pr，我会在做检阅后merge。

```bash
git push -u origin you_own-branch:you_own-branch
```

