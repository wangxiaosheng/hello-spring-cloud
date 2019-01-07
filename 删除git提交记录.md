### 删除git仓库所有提交历史记录，成为一个干净的新仓库
#### 1 Checkout

git checkout –orphan latest_branch

#### 2 Add all the files

git add -A

#### 3 Commit the changes

git commit -am “commit message”

#### 4 Delete the branch

git branch -D master

#### 5 Rename the current branch to master

git branch -m master

#### 6 Finally, force update your repository

git push -f origin master

###这是从网上摘的一段代码, 个人分析就是把所有代码放置到当前工作台, 之后删除所有历史, 再重新建MASTER分支. 这种方法对于主仓库可行, 但对于克隆仓库就失去了与主仓库的关联.