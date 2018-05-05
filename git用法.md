 写在一个地方好记些，不然时间一长习惯于依赖自动化工具就把命令什么的给忘了  
 --
### 1.注册，去掉引号就是查询当前状态  
git config --global user.name "tony"  
git config --global user.email "tony@gmail.com"

### 2.基本命令  
git init  
git add .  
git reset .  取消添加
git commit -m "first"  

git status  
git diff <dirname>      可以看到具体修改  
git checkout <dirname>  回滚没有添加的修改  

git log   
git log <commitid> -1 -p  查看一条记录的(-1)详细信息(-p)



### 3.用.gitignore文件建立忽略  

### 4.分支和远程仓库  
git branch v1 创建分支v1  
git checkout v1 切换分支到v1  
git merge v1 将v1分支和当前分支合并  
git branch -D v1 删除v1  

设https 为远程地址  

git clone https  
git push https master 同步到远程仓库master 分支  
git fetch https master 远程master 拉到本地隐藏分支（用git branch -a查看）
git diff <隐藏分支名> 查看远程和本地的不同  
git pull https master  下载远程并合并到本地
