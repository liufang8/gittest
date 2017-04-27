文件夹状态： 
	绿色对号： 已提交
	红色感叹号： 已经添加未提交
	红色加号： 为已添加

**add** 

# 添加当前文件夹
git add .  	

# 添加某个文件
git add <file> <file> 

# 添加某个文件
git add <dir> 

# 删除文件
git rm <file> 

# 改名文件
git mv file-origin file-renamed  


**checkout**
git checkout <file> //unstage to work dir

**reset**
# stage to unstage
git reset head <file> 

# 对工作区没有影响，撤销add增加到暂存区的内容
git reset
git reset head

# 撤销指定的文件
git reset -- filename
git reset head filename

# 重置暂存区和缓冲区，和上次提交一致
git rest --hard

# 切换到指定分支，并更新工作区
$ git checkout [branch-name]

windows下git add 时提示`warning: LF will be replaced by CRLF`
解决办法：git config --global core.autocrlf false
