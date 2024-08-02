## 拉取远程分支并进行线性合并
1. git pull origin master --rebase

## 补充：如果执行以上命令后，想回撤销合并退到之前的分支状态，按一下步骤：
## 1. 使用git reflog找到之前的提交记录
## 会看到类似以下输出：
## abc1234 (HEAD -> master) HEAD@{0}: rebase finished: returning to refs/heads/master
## def5678 HEAD@{1}: pull --rebase: checkout master
## ghi9012 HEAD@{2}: commit: Your previous commit message
## ...
## 找到你在执行 git pull --rebase 之前的提交哈希值（例如 ghi9012）
## 使用git reset --hard <commit-hash>命令即可