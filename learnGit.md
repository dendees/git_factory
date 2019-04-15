# GIT 使用

## 概念
1. 版本库（Repository）：本地git文件夹里的东西
2. 工作区：本地工作目录
3. 暂存区：git add后没有commit 的区域

## 常用命令
1. git init
2. git add docname : docname可以有多个，用空格分开，add以后添加到暂存区
3. git commit :提交暂存区的内容到版本库。生成一个版本，版本有commitID, HEAD
4. git reset : --hard commitID 回滚到某个版本
                --hard HEAD^ 回滚到上一个版本
5. git status: 状态查看
6. git checkout 工作区回滚到上次 git add/git commit 状态. 想把已经add的修改撤销，需要git reset HEAD docname
7. git rm docname 删除暂存区的文件
8. git remote add origin git@ <github的git文件地址>： 本地代码和github库建立关系
9. git push -u origin master : 推送本地库的内容至github