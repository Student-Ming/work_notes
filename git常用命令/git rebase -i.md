# 说明：该命令会进入文本编辑模式
## 操作说明：【i】进入编辑模式，【esc】退出编辑模式，【shift + :】进入指令模式，【wq】保存退出，【u】撤销，【shift+zz】强制退出
## 具体命令：git rebase -i  <commit_id>  或者 git rebase -i HEAD~次数
## git rebase --continue 让rebase继续，--abort 终止rebase操作
1. pick：保留该commit
2. reword：保留该commit，但需要修改该commit的注释
3. edit：保留该commit, 但要修改该提交(可以拆分更细的 commit)
4. squash：将该commit和前一个commit合并，两次注释都保留
5. fixup：将该commit和前一个commit合并，但不要保留该提交的注释信息
6. drop：丢弃该commit
## 应用场景：合并commit，修改历史commit信息，删除某个历史commit
## 注意：rebase会变更修改节点的<commit_id>，所以push的时候需要加上-f 强推，因此不能在公共分支上进行rebase操作（项目负责人除外）
