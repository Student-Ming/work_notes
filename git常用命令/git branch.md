## 删除分支
git branch -D <分支名>

## 重命名分支
git branch -M <老分支名> <新分支名>

## 将本地分支与远程分支关联
git branch --set-upstream-to=origin/xxx

## 取消本地分支与远程分支的关联
git branch --unset-upstream-to=origin/xxx

## 在git fetch origin后
## 查看所有远程分支
git branch -r
## 查看所有本地和远程分支
git branch -a