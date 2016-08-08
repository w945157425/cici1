# cici1
git命令学习 第一天
git是一个分布式版本控制系统

1.git init
  通过这个命令可以把当前目录变成Git可以管理的仓库
2.git add file
  把文件添加到仓库，准确的说是添加到了暂存区（stage）
3.git commit -m "description 版本描述"
  把文件提交到仓库
4.git status
  时刻掌握仓库的状态
5.git diff
  查看修改的具体内容
6.git log 
  查询版本历史记录
  git log --pretty=oneline
  简化后的历史记录
7.git reset
  重置版本
  git reset --hard HEAD^
  返回到上一个版本   
  HEAD^^代表上上个版本  HEAD~100代表往上100个版本
  git reset --hard commit_id
  commit_id 提交的版本号
8.git reflog
  用来记录每一次命令
9.git checkout -- file
  可以丢弃工作区的修改
10.git reset HEAD file
  可以撤销暂存区的修改
11.git rm 
  用于删除一个文件
12.ssh-keygen -t rsa -C "youreamil@example.com"
  用于创建SSH Key，会创建id_rsa和id_rsa.pub两个文件，这两个就是SSH Key的密钥对，id_rsa是私钥，id_rsa.pub
  是公钥。
13.git remote add origin git@github.com:username/repo-name.git
  关联一个远程仓库，这个远程仓库是在GitHub上创建的
14.git push -u origin master
  使用该命令第一次推送master分支的所有内容
15.git push origin master
  每次本地提交后，都可以使用该命令推送最新修改。
16.git clone git@github.com:username/repo-name.git
  从远程库克隆一个本地库。
17.git checkout -b dev
  创建并切换到名为dev的分支，相当于 git branch dev 和 git checkout dev;
18.git branch
  查看所有分支，当前分支前会标一个*号。
19.git checkout master
  切换回master分支
20.git merge dev
  把dev分支的工作成果合并到master分支上
21.git branch -d dev
  删除dev分支。
22.git log --graph --pretty=oneline --abbrev-commit
  查看分支情况 分支合并情况
23.git merge --no-ff -m "description版本描述" dev
  在禁用Fast forward的情况下合并dev分支到master分支。使用--no-ff可以看出来曾经做过合并
24.git stash
  可以把当前工作区暂时“储藏”起来，进行另外分支的操作
25.git stash list
  查看刚刚“储藏”的工作区
26.git stash pop 
  恢复工作区内容，并删除stash
27.git stash apply
  恢复工作区内容，但是并不删除stash
28.git stash drop
  删除stash
29.git branch -D name
  强行删除name分支  
30.git remote
  查看远程库的信息
31.git remote -v
  查看远程库的详细信息
32.git pull
  从远程抓取分支。
33.git checkout -b branch-name origin/branch-name
  在本地创建和远程分支对应的分支
34.git branch --set-upstream branch-name origin/branch-name
  建立本地分支和远程分支的关联
35.git tag <name>
  给最新的版本打上标签，便于理解，相当于软件的版本号
36.git tag <name> commit_id
  给commit_id的版本打上标签
37.git tag
  查看标签
38.git show <name>
  查看某个标签的详细信息
39.git tag -a <name> -m "description描述" commit_id
  创建带有说明的标签 -a指定标签名， -m指定说明文字
40.git tag -s <name> -m "description描述" commit_id
  通过-s用私钥签名一个标签
41.git tag -d <name>
  删除某个标签
42.git push origin <name>
  推送某个标签到远程
43.git push origin --tags
  一次性推送全部标签到远程
44.git tag -d <name> /git push origin :refs/tags/<name>
  要删除已经推送到远程的标签，首先删除本地标签，再删除远程标签。

                                                                                                   ----参考资料《Git教程》廖雪峰
