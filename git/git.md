# git基本命令

### 创建新仓库
 git init

### 检出仓库
 git clone
 git remote add origin

### 添加和提交
git add filename/git add *  
git commit -m "备注"

###更新
git pull

### 推送
git push origin master  
* 如果你还没有克隆现有仓库，并欲将你的仓库连接到某个远程服务器，你可以使用如下命令添加：  
* git remote add origin server
如此你就能够将你的改动推送到所添加的服务器上去了    

### 创建分支
 git branch 分支名
### 切换分支
 git checkout 分支名
### 查看分支
 git branch -a
### 删除分支
 git branch -d
### 删除远程分支
git push origin --delete remote_branch
###  将本地分支推送到远程
 git push origin 本地分支名:远程分支名

###合并分支
  切换到需要被合并的分支  
  git merge 别的分支名  
  冲突解决之后 --> git add  

### 查看差异
git diff 源分支 目标分支

### 标签  
git tag 标签名  
git push origin 标签名

### 替换本地改动
git checkout 文件名

### 假如你想要丢弃你所有的本地改动与提交，可以到服务器上获取最新的版本并将你本地主分支指向到它：
git fetch origin  
git reset --hard origin/master

## 有用的贴士
### 内建的图形化 git：
gitk

### 彩色的 git 输出：
git config color.ui true

### 显示历史记录时，只显示一行注释信息：
git config format.pretty oneline

### 交互地添加文件至缓存区：
git add -i
