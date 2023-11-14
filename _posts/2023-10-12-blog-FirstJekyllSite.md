---
layout: post
title: My First Jekyll Website
author: Ke Yi
categories: blog
tags: [Jekyll, Tech]
date: 2023-10-12 14:01 +0800
toc: true
---
The way to establish this website.
{: .message }

# 1. Why did I establish this website?
I established this site to share some experience, including but not limited to experimental techniques, software use, etc..

I'm looking forward to making this site bigger someday :>

# 2. How did I establish this website?
The process of building this site is roughly divided into three steps: building the Jekyll environment, building the web framework, and deploying to Github.

## 2.1 Build Jekyll environment
I chose to use Jekyll and Github Pages to build this site.

- First of all, Jekyll is based on a Ruby environment, and I used the Homebrew control tool Rbenv and installed Ruby through it.

<mark>P.S. Ruby version try to choose 2.7.2 version, such as version is too high part of the Jekyll template may not be compatible.</mark>

{% highlight zsh %}
brew rbenv
rbenv install 2.7.2
{% endhighlight %}

- Apply version 2.7.2 globally and source it to shell.

{% highlight zsh %}
rbenv global 2.7.2
source ~/.zshrc
{% endhighlight %}

- Further installing jekyll via gem allows you to start building the web framework.

{% highlight zsh %}
gem install jekyll bundler
{% endhighlight %}


### 2.2 Creating a web framework
There are two main ways to build a web framework, Jekyll can directly build a minima theme website template.

{% highlight zsh %}
jekyll new mywebsite
{% endhighlight %}

In addition, you can also fork existing templates. This site is mainly based on the Jekyll theme [not-pure-poole](https://github.com/vszhub/not-pure-poole)

<mark>P.S. The following operations are need to cd to the Jekyll root directory first</mark>

When you fork the template, you should use bundle to install the gem used in the template before deploying the server for the first time, and then use the serve command to deploy the server locally.

{% highlight zsh %}
//Install the gem
bundle install
//Deploy the server locally
bundle exec jekyll serve
{% endhighlight %}

Then you can access the local website at [http://localhost:4000](http://localhost:4000)

## 2.3 Deploying to Github Pages
When debugging is complete, you can deploy to Github Pages via Github desktop.

First, you need to create a repository in the Github repository named (username).github.io, e.g. keyi926.github.io.

Clone the repository locally and copy the debugged website files to the Github directory, submit the update in Github Desktop and push it to Github server.

Then you can access the website via [keyi926.github.io](http://keyi926.github.io)
