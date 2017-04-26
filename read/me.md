文件夹状态： 
	绿色对号： 已提交
	红色感叹号： 已经添加未提交
	红色加号： 为已添加

**add** 
git add * //添加所有 	
git add <file> //添加某个文件


**checkout**
git checkout <file> //stage to unstage

**reset**

git reset head <file> //change to unstage


Total 6143 (delta 833), reused 2524 (delta 833)?

windows下git add 时提示`warning: LF will be replaced by CRLF`
解决办法：git config --global core.autocrlf false
