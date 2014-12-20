---
layout: post
title: "如何使用emacs"
date: 2014-12-20 11:44:35 +0000
comments: true
categories:
---

今天闲着没事，又上我们的[ncuopen](https://github.com/ncuopen)上面看了一下，发现小组现在活动极其不频繁，首页和wiki都没有怎么更新，然后上irc上看了一下，发现也没有人在线。
> 一个开源社区最大的悲哀就是没有活跃的用户，没有一个持续贡献的志愿者团队。

加入小组这么久了都没有做什么贡献真是惭愧，今天想了一下我可以整理一下我对于emacs使用的一点小小的心得。以下将会简单的说说我平时使用emacs来干什么。

1. 写代码，这是最基本的功能。
2. 上网，在emacs24之前的版本必须使用一个叫做`emacs-w3m`的第三方扩展才能在emacs里面上网，但是现在emacs自己做了一个基于elisp写的文本浏览器`eww`，使用方式也很简单，直接`M-x eww`然后输入要搜索的内容或者是要打开的url就行，现在`eww`默认的搜索引擎是`duckduckgo`。
3. 聊天，今天上`#ncuopen`上看了一下，发现聊天室里面没人在，突然比较一下那些比较火的聊天室，如`ubuntu`, `debian`每天上去都会有一大堆人在线，随便说一句话就会被别人刷屏，差距真的很大。如果要在emacs里面使用irc聊天，可以使用`erc`来连接服务器。
4. 看pdf，emacs内建是可以打开pdf文件的，如果习惯了emacs的快捷键，而且不喜欢在`evince`，`okular`下面必须使用鼠标的操作，那么可以试试用emacs看pdf。
5. 写博客，我自己也在github上面搭了一个octopress的博客，在本地就是用emacs编辑的博客，因为emacs支持`markdown`语法，编辑的时候可以直接看到语法高亮，保存后可以在本地预览。
6. 执行shell命令，要么是使用`M-x shell`来打开一个shell或者是`M-x eshell`来使用emacs自带的终端模拟器，我喜欢用后者，然后就可以运行任何的shell命令了。不过我用eshell用得少，平时都是在`urxvt`里面执行命令的。
7. 执行解释器，很动语言都内建了一个elpa的解释器，如ruby, python, php, haskell，sml等，如果想尝试一下某个表达式或者是某个代码段又不想写一个测试文件，那么在解释器里运行是最方便的了，执行`M-x run-python`, `M-x run-haskell`，会打开对应语言的解释器，就像在终端执行一样。如果想获得更多语言的支持，可以去[elpa](http://elpa.gnu.org/packages/)或者是[melpa](http://melpa.org/)上面找找。
8. 使用git，emacs有个扩展叫做`magit`，用它来提交代码，查看差异，查看版本比在终端使用git命令方便。
9. 看图，这个功能估计很少人会用，`display`和`feh`已经做得很棒了。

如果要使用上面的功能，最好使用[prelude-emacs](https://github.com/bbatsov/prelude)上面的配置，省去很多配置的麻烦。

另外我发现现在小组没有一个好的交流的地方，在github上面提issue总是不太方便，找到了一个开源项目[esotalk](https://github.com/esotalk/esoTalk)可以很方便的用来搭建论坛，不知道有没有小伙伴愿意贡献一下。
