## Git操作常用指令

### **Git操作指令**

1. git init 初始化一个git 仓库
2. git add test.txt 添加一个文件到仓库，可以添加多个，一空格隔开
3. git commit -m “remarks” 把文件提交到仓库
4. git status 当前仓库的状态
5. git remote 查看远程库的信息
6. git remote -v 查看上传协议 SSH/HTTPS
7. git remote 
8. git reset --hard HEAD^　　把当前版本回退到上一个版本
9. git rm <file>  
10. git push -u origin master
11. 分支操作

```
    git branch juziBranch   创建分支juziBranch　　git checkout     	     juziBranch  切换分支
　　Switched to branch 'juziBranch'  提示信息 
　　相当于 git checkout -b juziBranch   创建并切换到分支
　　git branch  查看所有的分支信息 ，当前分支前带有*
　　git branch –all   查看所有的分支信息
　　git checkout master  切回主分支
　　git merge juziBranch  合并juziBranch分支到主分支master上
　　git branch -d juziBranch  删除juziBranch本地分支
　　git push origin :juziBranch  删除远程库上的分支
　　git push branch juziBranch  push本地分支juziBranch到远程库
　　git push origin master   把该分支上的本地提交推送到远程库
    git push origin branchName　　推送其他分支
```

 更新当前分支   git pull

本地提交 git commit -am
　　当你本地的文件都已经用git add “” 或之前已经添加到缓存区后，这时本地文件有所改动(修改过的或新加入的)，需要进行commit 提交，使用git commit -am “remark”即可全部提交到staged，最后 git push到远程库。
　　**注意**：在分支切换之前最好先commit全部的改变，除非你真的知道自己在做什么哦

 添加所有的 git add -A
 不再需要一个个的单独添加

追踪未添加的文件git add . 
     git add . 不但可以跟单一文件，还可以跟通配符，更可以跟目录。一个点就把当前目录下所有未追踪的文件全部add了 

git reset HEAD a.txt 撤销暂存的文件 （已经添加到暂存区了）

配置使用用户

```
    git config --global user.name ‘橘子太酸辣’
    git config --global user.email designbyly@aliyun.com
```

　　git config --global 参数 ，这个参数就是你机器上的git仓库都会使用这个配置，否则你就只能对某个仓库指定不同的用户名和邮箱

先写到这里关于命令行的操作，更多请联系本人邮箱designbyly@aliyun.com

