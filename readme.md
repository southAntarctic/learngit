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
分支：
	查看分支： git branch
	创建分支： git branch <name>
	切换分支： git checkout <name>
	创建+切换分支： git checkout -b <name>
	合并分支到当前分支： git merge <name>
	删除分支： git branch -d <name>
	分支冲突解决方案： 把 git 合并失败的文件手动编辑为我们希望的内容，再提交。
	查看分支合并图： git log --graph

	do some test
