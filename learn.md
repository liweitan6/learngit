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
* `git rm` 将工作区文件删除并将删除提交到暂存区
* `git checkout -- <file>` 用版本库的版本替换工作区的版本
* 