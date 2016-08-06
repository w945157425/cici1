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
                                                                                                     ----参考资料《Git教程》廖雪峰
