# Git学习笔记

## 设置

项目级别/仓库级别：仅当前本地库范围内生效。
- git config user.name/user.email sjx/sijianxin01@163.com

系统用户级别：登录当前操作系统的用户范围生效。
- git config --global user.name/user.email sjx/sijianxin01@163.com

## 基本操作

项目初始化。
- git init

查看状态。
- git status

添加追踪(将文夹加入提交缓存区)命令。
- git add <filename>

解除追踪命令。
- git rm --cached <filename>

提交(从缓存区提交到本地库)命令。
- git commit <filename>
- git commit -m "message" <filename>

打印日志命令。
- git log 

打印单行日志。
- git log --pretty=oneline

比较工作区和暂存区文件差异命令。
- git diff 'filename'

## 分支操作

查看分支命令：git branch -v

创建分支命令：git branch 'branchname'

切换分支：git checkout 'branchname'

分支合并命令：git merge ‘otherbranchname’

## 远程仓库

查看当前本地别名命令：git remote -v

添加别名：git remote add '别名' '地址'

推送：git push '地址' '分支'

克隆命令：git clone '远程库地址'

更新本地：git fetch '地址' ‘分支’ or git merge '地址'/‘分支’ or git pull '地址' ‘分支’(无需检出)
