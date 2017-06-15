---
title: git
date: 2017-06-15 15:50:42
tags:
---

1. 拉取远程分支到本地
```
git fetch upstream Dev2.4:2.4
```
2. stash储藏
```
git stash list
git stash apply stash@{0}
git stash drop stash@{0}
```
3. 合并冲突
1）重命名
```
git rm --cached
git commit
git add .
git commit
```
