title: git常用操作
tags:
  - git
categories:
  - Git
date: 2020-08-19 15:41:00
---
>### 常见操作命令 

初始化一个Git仓库 git init

查看分支：git branch

创建分支：git branch <name>
  
切换分支：git checkout <name>
  
<!--more-->
  
创建+切换分支：git checkout -b <name>
  
合并某分支到当前分支：git merge <name>
  
删除分支：git branch -d <name>
  
查看远程库信息 git remote -v；

从本地推送分支 git push origin branch-name，如果推送失败，先用git pull抓取远程的新提交；

在本地创建和远程分支对应的分支 git checkout -b branch-name origin/branch-name，本地和远程分支的名称最好一致；

建立本地分支和远程分支的关联 git branch --set-upstream branch-name origin/branch-name；

从远程抓取分支 git pull，如果有冲突，要先处理冲突。

工作区的状态 git status命

查看修改内容 git diff

版本回滚 git reset --hard commit_id

查看提交历史 git log 查看命令历史 git reflog 


>### 删除文件操作 

$ git pull origin master 将远程仓库里面的项目拉下来

$ dir  查看有哪些文件夹

$ git rm -r --cached target  删除target文件夹

$ git commit -m '删除了target'  提交,添加操作说明

$ git push -u origin master 将本次更改更新到github项目上去

>### 合作开发 fork操作

![Audits - Lighthouse](https://lemon-29-zl.oss-cn-beijing.aliyuncs.com/Blog/github.png)