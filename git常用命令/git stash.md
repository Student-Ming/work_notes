## 把本地的改动缓存起来
git stash

## 缓存代码时添加备注，便于查找。强烈推荐
git stash save "message"

## 查看缓存记录
git stash list

## 取出上一次缓存的代码，并删除这次缓存
git stash pop

## 取出 index 为2缓存代码，并删除这次缓存，index 为对应 git stash list 所列出来的
git stash pop stash@{2}

## 取出上一次缓存的代码，但不删除这次缓存
stash apply

## 取出 index 为2缓存代码，但不删除缓存
git stash apply stash@{2}

## 清除某次的缓存
git stash drop stash@{n}

## 清除所有缓存
git stash clear
