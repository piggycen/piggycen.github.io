---
layout:     post
title:      搭建Rails+Mongoid环境
date:       2016-03-01
summary:    在Rails工程中运用mongoid
categories: rails
---

在Rails工程中运用Mongoid，和Active Record一样，Mongoid是一个基于MongoDB的比较不错的ORM框架。

Active Record只支持关系型数据库，MongoDB是一个基于分布式存储的数据库，介于关系型数据库和非关系型数据库之间，是非关系型数据库中功能比较丰富，比较像关系型数据库的一种。如果需要在Rails中使用MongoDB，可以安装第三方的gem库。


##安装Gem

首先需要安装Mongoid的gem包

	gem install mongoid

<br>
然后在自己的Rails工程的Gemfile文件中添加一下代码

	gem 'mongoid', '~> 5.1.0'

<br>
使用自动生成代码，生成Mongoid的配置文件，执行完之后会在app/config目录下生成一个yml文件，mongoid.yml

	rails g mongoid:config

<br>
orm对象关系映射，把程序中的对象和关系型数据库中的数据表联系起来，程序中对象的属性和对象之间的关系可以通过一种简单的方法从数据库中获取，无需直接编写SQL语句，也不会过度依赖特定的数据库种类。

最后需要告诉Rails，这个工程使用的orm是Mongoid，所以需要在application.rb文件中添加一下代码块。

	congig.generators do |g|
	  g.orm :mongoid
	end





