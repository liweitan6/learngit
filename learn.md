* `git init` 将当前目录变成Git管理的仓库  
* `git add <file>` 将工作区加入到暂存区  
* `git commit -m <"message">` 将暂存区提交到版本库
* `git status` 查看仓库当前状态
* `git diff` 
    * `git diff <file>` 记录上次add后的变动
    * `git diff --cached <file>` 记录上次commit后的变动
    * `git diff HEAD -- <file>` 将当前提交版本与工作区对比
* `git log` 查看提交历史，可以加上` --pretty=oneline` 简化信息
* `git reflog` 查看命令历史，以确定回到未来的哪个版本
* `git reset`
    * `git reset --hard <commit_id/HEAD^>` 根据id或HEAD<^>进行版本回退
    * `git reset HEAD <file>` 将暂存区的修改撤销，放回工作区
* `git rm` 将工作区文件删除并将删除提交到暂存区（工作区与版本库一致）
* `git checkout -- <file>` 用版本库的版本替换工作区的版本  
  
    `git rm -> git checkout` no  
    `git rm -> git reset HEAD -> git checkout` yes

* `git remote add origin git@server-name:path/repo-name.git` 关联远程库，远程库名为"origin"
* `git push -u origin master` 第一次用该命令推送master分支内容，此后使用`git push origin master`
* `git remote -v`查看远程库信息
* `git remote rm <repo_name>` 删除远程库
* `git clone git@server-name:path/repo-name.git` 克隆远程库到当前文件夹下
* `git branch` 查看分支
* `git branch <name>` 创建分支
* `git checkout <name> / git switch <name>` 切换分支
* `git checkout -b <name> / git switch -c <name>` 创建并切换分支
* `git merge <name>` 合并某分支到当前分支
* `git branch -d <name>` 删除分支


