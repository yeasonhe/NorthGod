---
layout: post
title: 一些有用的Git命令组合
---

# 一些有用的Git命令组合
![](http://ww1.sinaimg.cn/large/ee21033aly1fwj4i49ny3j21hc0xc78j.jpg)
[@我的微博](https://weibo.com/yeasonhe)
[@个人博客](https://staroflion.github.io/)

### 关于使用策略
目前比较好的Git分支的策略可以参考:
[Vincent Driessen](https://nvie.com/)提出了一个非常值得借鉴的[策略](https://nvie.com/posts/a-successful-git-branching-model/)
同时可以参考[阮一峰](http://www.ruanyifeng.com)的[git分支管理策略](http://www.ruanyifeng.com/blog/2012/07/git.html),相当于是上篇文章的翻译版。

### 关于`git add` 命令的含义

### 重命名远程分支

分为以下`三个`步骤:

- 先删除远程分支(product)

    ```sh
    git push --delete origin product
    ```
- 然后重命名本地分支

    ```sh
    git branch -m product dev
    ```
- 最后把重新命名好的本地分支推送到origin

    ```sh
    git push origin dev:dev
    ```


[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [@我的微博]: <https://weibo.com/yeasonhe>
