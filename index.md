---
layout: page
category : tutorial
title: Beginning of Blog
tagling: build Blog By Jekyll Bootstrap
tags: [Jekyll]
---
{% include JB/setup %}



之前一直用印象笔记记录各方面的心得，只是自己看，所以比较零散。
为了给自己点定期整理的动力，所以计划在GitHub上创建自己的Blog。

下面是自己创建GitHub Blog过程，希望可以为有类似需求的Geek提供帮忙

## GitHub Pages
    

>依据官方的[Github Pages](https://pages.github.com/)指导

### 创建命名为*username.github.io*的Repository
    

###在Repository下创建`index.html`
#####文件内容:
	<!DOCTYP html>
    <html>
    	<body>
    		<h1>Hello World</h1>
    	    <p>I'm hosted with GitHub Pages.</p>
    	</body>
    </html>
    
将`index.html`push到**GitHub**，访问<http://username.github.io>即可看到效果

##利用Jekyll创建本地MarkDown格式Blog
写HTML格式的Blog时，相当的时间用在了HTML语法上。**MarkDown**的语法相对*HTML*更简单，但是个人感觉更合适写作。

准备使用**GitHub**推荐的`Jekyll`来搭建本地Blog服务器，[Jekyll](http://jekyllcn.com/)是将纯文本转化为静态博客网站的Ruby Gem

###本机环境是OS X，虽然系统自带Ruby，但是因为系统本身需要使用到Ruby，所以为了不影响系统不能Ruby来安装Jekyll。为了解决这个问题，所以先安装[RVM](https://rvm.io/)（Ruby Version Management）
    $ \curl -sSL https://get.rvm.io | bash -s stable
###安装当前最新版本的Ruby并使用
    $ rvm list known
    $ rvm install 2.1.2          //安装Ruby2.1.2
    $ cd /username.github.io     //进入本地Blog路径
    $ rvm use 2.1.2              //使用安装的Ruby2.1.2
    $ rvm gemset create blogRubyGem //创建Jekyll的RVM GemSet
    $ rvm gemset use blogRubyGem //当前路径下使用myBlogRubyGem这个GemSet
    
>###依据[官方指导](官方指导)安装Jekyll


##安装Jekyll的模板
上面完成了本机搭建Jekyll的环境，但是还没有符合Jekyll规则的网站架构。当然可以依据Jekyll官方的文档搭建一个，但是我这里使用了当前比较容易上手的主题Jekyll Bootstrap来搭建自己的Blog。
因为过程比较简单，所以具体的流程请访问官网：<http://jekyllbootstrap.com/>

##最后推荐一个OS X的免费MarkDown编辑器[Mou](http://mouapp.com/)
![Mou](http://mouapp.com/images/Mou_Screenshot_1@2x.png)
    
   
	
	