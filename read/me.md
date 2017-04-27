文件夹状态： 
	绿色对号： 已提交
	红色感叹号： 已经添加未提交
	红色加号： 为已添加

**add** 
git add . //添加当前文件夹 	
git add <file> <file> //添加某个文件
git add <dir> //添加某个文件
git rm <file>  //删除文件
git mv file-origin file-renamed 改名文件 


**checkout**
git checkout <file> //stage to unstage

**reset**
# change to unstage
git reset head <file> 


# 切换到指定分支，并更新工作区
$ git checkout [branch-name]

Total 6143 (delta 833), reused 2524 (delta 833)?

windows下git add 时提示`warning: LF will be replaced by CRLF`
解决办法：git config --global core.autocrlf false
