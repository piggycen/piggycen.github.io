---
layout:     post
title:      如何在Sublime text2中编译CoffeeScript
date:       2016-03-17
summary:    在Sublime text2中编译Coffee文件
categories: Sublime
---

## 方法一：修改CoffeeScript.sublime-build文件

![sublime preferences](/images/sublime_preferences.png)

在此目录下找到位于CoffeeScript文件夹下的CoffeeScript.sublime-build文件

修改前为

![build before](/images/build_before.png)

-----

修改后为

![build after](/images/build_after.png)

----

按上例修改完成后，快捷键shift+command+b，就可以在控制台输出编译后的JavaScript代码

注：以上均在Mac OS系统下，在Windows下，网上的解决方法是还需将"coffee"修改为"coffee.cmd"

"-cp": compile and  print， 编译并打印，此命令可参考coffee -h的命令帮助

![coffee help](/images/coffee_help.png)

## 方法二：安装Package----coffee compile

顾名思义coffee compile即编译Coffee文件，具体安装过程可参考github项目--[sublime-coffee-compile](https://github.com/surjikal/sublime-coffee-compile)

安装完成之后，快捷键shift+control+c

方法二较方法一的优势在于，在方法二中可以自主选择coffee文件中的一段代码进行编译，并且高亮显示，视觉效果比较好

### 方法一编译结果

![compile first](/images/compile_first.png)

### 方法二编译结果
![compile second](/images/compile_second.png)





