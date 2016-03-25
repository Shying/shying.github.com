---
layout: post
title: "How to build a blog"
tagline: "github page & jekyll"
description: "how to build a static blog"
category: study
tags: [jekyll]
---
{% include JB/setup %}

首先，参考链接[http://jekyllbootstrap.com/usage/jekyll-quick-start.html](http://jekyllbootstrap.com/usage/jekyll-quick-start.html)

这是jekyllbootstrap，里面有bootstrap和twitter模板，当然也可以使用原生的jekyll，参考链接[https://help.github.com/articles/setting-up-your-pages-site-locally-with-jekyll/](https://help.github.com/articles/setting-up-your-pages-site-locally-with-jekyll/)

我是在windows7里面搭建的本地环境，过程与jekyllbootstrap quick start一致，不过过程中遇到点问题：


- #### gem安装jekyll提示ssl问题 ####

>执行如下命令：
>
>gem source -r https://rubygems.org/
>
>gem source -a http://rubygems.org/


- #### 提示requires installed build tools ####

>参考[Installing Jekyll on Windows](http://flatshaded.com/2013/05/installing-jekyll-on-windows/)进行安装

- ### 提示cannot load such file -- pygments ###

>参考[stackoverflow](http://stackoverflow.com/questions/33439019/jekyll-serve-didnt-work-it-looks-like-you-dont-have-pygments-or-one-of-its-dep)
>gem install pygments.rb
>gem 'pygments.rb'

- #### jekyll serve后，assert找不到 ####

>修改根目录下_config.yml文件，里面的ASSET_PATH修改为/assets/themes/bootstrap-3（自己在assert目录下看一看目录到底是什么样子的）

###关于主题 ###

知乎上有关于jekyll themes的话题，[GO](https://www.zhihu.com/question/20223939)

啦啦啦 一大堆主题来袭！[Jekyll Themes](http://jekyllthemes.org/)