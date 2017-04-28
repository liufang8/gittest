文件夹状态： 
	绿色对号： 已提交
	红色感叹号： 已经添加未提交
	红色加号： 为已添加

**init**
# 在当前目录新建一个Git代码库
$ git init

# 新建一个目录，将其初始化为Git代码库
$ git init [project-name]

# 下载一个项目和它的整个代码历史
$ git clone [url]


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


**commit**

# work dir to repository
git commit -a 

# see diff info
git commit <file> -v

**branch**

# 列出所有本地分支
$ git branch

# 列出所有远程分支
$ git branch -r

# 列出所有本地分支和远程分支
$ git branch -a

# 新建一个分支，但依然停留在当前分支
$ git branch [branch-name]

# 把本地分支发布到远程分支
$ git push origin [branch-name]

# 新建一个分支，并切换到该分支
$ git checkout -b [branch]

# 新建一个分支，指向指定commit
$ git branch [branch] [commit]

# 新建一个分支，与指定的远程分支建立追踪关系
$ git branch --track [branch] [remote-branch]

# 切换到指定分支，并更新工作区
$ git checkout [branch-name]

# 切换到上一个分支
$ git checkout -

# 建立追踪关系，在现有分支与指定的远程分支之间
$ git branch --set-upstream [branch] [remote-branch]

# 合并指定分支到当前分支
$ git merge [branch]

# 选择一个commit，合并进当前分支
$ git cherry-pick [commit]

# 删除分支
$ git branch -d [branch-name]

# 删除远程分支
$ git push origin --delete [branch-name]
$ git branch -dr [remote/branch]

# 切换到指定分支，并更新工作区
$ git checkout [branch-name]

# 在当前版本，创建远程分支，更新
$ git pull origin branch_name




**配置**
git config --global core.autocrlf false

windows下git add 时提示`warning: LF will be replaced by CRLF`
解决办法：git config --global core.autocrlf false
