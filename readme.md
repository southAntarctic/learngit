初始化：
	初始化仓库： git init
	添加文件到仓库： git add <file>
	提交： git commit -m <message>
基本操作：
	查看状态： git status
	查看不同： git diff <file>
	查看历史纪录： git log
	版本回退： git reset --hard HEAD^ 
	查看历史命令： git reflog
	丢弃工作区修改： git checkout -- file
	暂存区复原： git reset HEAD <file>
	删除文件： git rm
远程库：
	关联远程库： git remote add origin git@server-name:path/repo-name.git
	第一次推送master分支所有内容： git push -u origin master
	推送最新修改： git push origin master 
	查看远程库信息： git remote -v
	本地推动分支： git push origin branch-name
		若推送失败先抓取远程的新提交： git pull
	在本地创建和远程分支对应的分支： git checkout -b branch-name origin/branch-name (名称最好一致)
	建立本地分支和远程分支的关联： git branch --set-upstream branch-name origin/branch-name
	从远程抓取分支： git pull
	把本地未 push 的分叉提交历史整理成直线： git rebase
分支：
	查看分支： git branch
	创建分支： git branch <name>
	切换分支： git checkout <name>
	创建+切换分支： git checkout -b <name>
	合并分支到当前分支： git merge <name>
	删除分支： git branch -d <name>
	分支冲突解决方案： 把 git 合并失败的文件手动编辑为我们希望的内容，再提交。
	查看分支合并图： git log --graph
	隐藏工作现场： git stash
	恢复工作现场： git stash pop
	丢弃未合并过的分支： git branch -D <name>

标签:
	新建标签：git tag <tagname> 默认为HEAD ，也可指定commit id 
	指定标签信息： git tag -a <tagname> -m "xxx"
	查看所有标签： git tag
	推送本地标签： git push origin <tagname>
	推送全部未推送过的本地标签： git push origin --tags
	删除一个本地标签： git tag -d <tagname>
	删除一个远程标签： git push origin :refs/tags/<tagname>
	

	do some test
