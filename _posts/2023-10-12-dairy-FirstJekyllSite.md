---
layout: post
title: My First Jekyll Site
author: Ke Yi
tags: [Jekyll, Tech]
date: 2023-10-12 14:01 +0800
toc: true
---
欢迎来到本站！
{: .message }

## 1.建站目的
建立此个站的初衷是为了分享一些心得体会，包括但不限于实验技术，软件使用等。

希望有朝一日能将小站做大做强:>

## 2.建站流程
建立此站的过程大致分为搭建Jekyll环境、建立网页框架、部署到Github三个步骤。

### 2.1 搭建Jekyll环境
本站选择使用Jekyll和Github Pages来搭建。原因其一是这个方案完全免费，其二是因为Jekyll所提供的静态页面完全满足我的轻度使用。

- 首先，Jekyll基于Ruby环境，我使用了Homebrew控制工具Rbenv并通过其安装Ruby。

<mark>特别注意，Ruby版本尽量选择2.7.0版本，如版本过高部分Jekyll模板可能不兼容。</mark>

{% highlight zsh %}
brew rbenv
rbenv install 2.7.0
{% endhighlight %}

- 全局应用2.7.0版本，并source到shell。

{% highlight zsh %}
rbenv global 2.7.0
source ~/.zshrc
{% endhighlight %}

- 再进一步通过gem安装jekyll后可以开始建立网页框架。

{% highlight zsh %}
gem install jekyll bundler
{% endhighlight %}


### 2.2 建立网页框架
建立网页框架的方式主要有两种，Jekyll可以直接建立一个minima主题的网站模板。

{% highlight zsh %}
jekyll new mywebsite
{% endhighlight %}

此外,也可以fork已有的模板。本站主要基于Jekyll主题[not-pure-poole](https://github.com/vszhub/not-pure-poole)

<mark>之后的操作需要先cd到Jekyll网站根目录</mark>

当fork别人的模板时，初次部署服务器前应当使用bundle安装模板中使用的gem，之后使用serve命令在本地部署服务器。

{% highlight zsh %}
//安装缺失的gem
bundle install
//部署服务器到本地
bundle exec jekyll serve
{% endhighlight %}

之后便可以通过[http://localhost:4000](http://localhost:4000)访问本地网站

### 2.3 部署到Github
当调试完成后，可以通过Github desktop部署到Github Pages

首先需要在Github仓库中建立一个仓库，命名为（用户名）.github.io, 如keyi926.github.io

将该库克隆到本地，并将调试好的网站文件复制到Github目录下,在Github Desktop提交更新并push

便可以通过[keyi926.github.io](http://keyi926.github.io)访问网站
