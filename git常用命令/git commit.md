## 当前提交对上次提交记录进行覆盖
1. git commit -m "new message" --amend

## 一次性从工作区提交到本地仓库，相当于 git add . + git commit -m
## 此命令对未跟踪的文件无效
2. git commit -am "new message"

## 更改上次提交记录的文本信息
3. git commit --amend

## 跳过commit信息填写
4. git commit --amend --no-edit

# 跳过校验直接提交，很多项目配置 git hooks 验证代码是否符合 eslint、husky 等规则，校验不通过无法提交
## 通过 --no-verify 可以跳过校验（为了保证代码质量不建议此操作）
5. git commit --no-verify -m "commit message"
