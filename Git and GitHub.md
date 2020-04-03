# Git and GitHub

官网下载Git并安装，在GitHub注册，在想要下载仓库的地方右键进入Git Bash Here.

## 1.设置用户名和邮箱

git config --global user.name "GitHub用户名"

git config --global user.email "GitHub邮箱名"

## 2.在GitHub账号创建一个新仓库

## 3.克隆远程仓库到本地

git clone https://github.com/username/仓库名

若是出错，可以将https改为git(但是push那里会出错)

## 4.在本地仓库做一些增删改

touch a.txt

可以直接在本地工作区里面修改，使用命令亦新建文件。

## 5.查看仓库中文件的状态

git status

## 6.将工作区的更改提交到暂存区

git add/rm file

如 git add /rm a.txt代表增加/删除a.txt这个文件,若是多个文件，可直接写“git add ."

## 7.将暂存区的更改提交到本地仓库

git commit -m "message"

若提交一个文件，message可以写文件名（不太严格），如 add a.txt;多个文件时，可以只写一个。

## 8.将本地仓库的更改同步到远程仓库

git push (origin master)           括号里面内容可以不写

## 9.push时需要输入用户名和密码，先运行下面的命令，可以记录密码，以后push免密

git config --global credential.helper store

**注意：如果最新代码与本地不同，push会报错，每次push前先”git pull"以将最新文件下载下来，再push**