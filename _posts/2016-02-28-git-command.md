---
layout:     post
title:      git常用命令
date:       2016-02-28
summary:    git命令
categories: git
---
![git work](/images/git_work.png)

## git clone
`git clone <远程代码仓库网址> (<本地目录名>)`
<br><br>
会从远程仓库克隆一份代码到本地，一般本地仓库名和远程仓库名一致，想改变本地仓库名可加<本地目录名>

***

## git fetch
`git fetch <远程主机名> (<分支名>)`
<br><br>
从远程主机取回(所有分支/某分支)的更新

***

## git pull
`git pull <远程主机名> <远程分支名> : <本地分支名>`
<br><br>
取回远程主机某个分支的更新，并且和本地的特定分支合并
`git pull == git fetch + git merge`

***

## git status
`git status`
<br><br>
查看当前状态下变更的文件

***

## git add
`git add .`
<br><br>
添加当前所有变更的文件到暂存区
<br><br>
`git add [file1][file2]...`
<br><br>
将具体的文件添加到暂存区
<br><br>
`git add [dir]`
<br><br>
将具体的目录添加到暂存区

***

## git commit
`git commit -m [修改内容描写]`
<br><br>
将暂存区内的修改内容提交到远程仓库，并且为这次修改取名
