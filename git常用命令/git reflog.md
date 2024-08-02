# 作用：用于显示引用日志。它记录了所有对引用（如分支、HEAD 等）所做的更改，包括那些可能不会出现在 git log 中的更改。git reflog 主要用于查看和恢复到之前的状态，特别是在你需要撤销某些操作时非常有用

## 命令：git reflog
## 输出示例：
## abc1234 (HEAD -> master) HEAD@{0}: commit: Add new feature
## def5678 HEAD@{1}: checkout: moving from feature-branch to master
## ghi9012 HEAD@{2}: commit: Fix bug in feature
## jkl3456 HEAD@{3}: rebase: checkout master

## 常用场景：
## 恢复误操作：如果你误操作了某些命令（如 git reset 或 git rebase），可以使用 git reflog 找到之前的状态并恢复。
## 查看所有引用变动：包括那些不会出现在 git log 中的变动，如 checkout、reset、rebase 等。
