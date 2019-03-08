# 新行程开启，\(^o^)/
# 本地仓库上传到git流程
1.建立本地仓库.git；
# （$ git init）
2.将需要提交的本地文件复制与到本地仓库所在文件夹，但不是.git内；
3.将要提交的本地文件添加到本地仓库；
# （$ git add .）
4.新建提交文件版本说明；
# （$ git commit -m "loading first time"）
5.提交本地文件到仓库步骤如下：
# 1）$ git remote add origin （链接到要提交的仓库地址）
# 2）$ git remote add origin https:.../xiaobaiBk（如果有分支，链接）
# 3）$ git push -u origin master（可直接在当前仓库提交）

# 新建一个分支
1.新建分支
# $ git checkout -b xiaobaiOne
2.删除分支
# $ git checkout -d xiabaiOne
3.提交分支
# $ git push origin xiaobaiOne

# 查看远程仓库
1.查看远程都有哪些仓库
# $ git remote -v

# 从远程仓库将文件更新到本地
1.新建一个临时分支并将远程文件更新到这个分支
# $ git fetch origin master:temp 
2.切换到主干
# $ git checkout master
3.比较分支和主干的区别
# $ git diff temp
2.合并
# $ git merge temp
3.如果不想要temp分支了，可以删除此分支
# $git branch -d temp
