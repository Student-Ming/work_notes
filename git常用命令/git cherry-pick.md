## 将 commit-sha1 的变动合并至当前分支
git cherry-pick commit-sha1

## 只复制提交代码，需要自己手动提交
git cherry-pick -n <commit_id>

## 将多次 commit 变动合并至当前分支
git cherry-pick commit-sha1 commit-sha2

## 将 commit-sha1 到 commit-sha5 中间所有变动合并至当前分支（前开后闭）
git cherry-pick commit-sha1..commit-sha5

## pick 时解决冲突后继续 pick
git cherry-pick --continue

## 多次 pick 时跳过本次 commit 的 pick 进入下一个 commit 的 pick
git cherry-pick --skip

## 完全放弃 pick，恢复 pick 之前的状态
git cherry-pick --abort

## 未冲突的 commit 自动变更，冲突的不要，退出这次 pick
git cherry-pick --quit
