# 新行程开启，\(^o^)/
# 本地仓库上传到git流程
1.建立本地仓库.git；
# $ git init
2.将需要提交的本地文件复制与到本地仓库所在文件夹，但不是.git内；
3.将要提交的本地文件添加到本地仓库；
# $ git add name(这是文件夹的名字或者是文件，如果是文件夹前面要带一个/xiaobai,这样会把这个文件夹下面所有文件都提交，如果是文件就只提交这一个文件
#  $ git add -A 提交所有文件到本地缓存
4.新建提交文件版本说明；
# $ git commit -m "loading first time"
# $ git commit -am "loading first time" 提交全部代码，到本地资源库
5.提交本地文件到仓库步骤如下：
# 1）$ git remote add origin （链接到要提交的仓库地址）
# 2）$ git remote add origin https:.../xiaobaiBk（如果有分支，链接）
# 3）$ git push -u origin master（可直接在当前仓库提交）这个方式会覆盖掉远程仓库代码，不建议使用
# 4）提交方式：git push --set-upstream origin master  这个是第一次提交
# 5）提交方式：git push 这是本地修改后提交；
# 6）更新方式：git pull 这是拉取远程服务器最新代码；
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
