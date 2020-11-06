# test_git_remote
To test the configuration

I'm learning how to use a remote git repository.

This file is created on-line then modified locally.

使用
`git remote add shorname url`
创建一个短名，来代替远程仓库的名称（网址、用户名、仓库名）

例如
`git remote add test git@github.com:EvannaLynch/test_git_remote.git`
则以后test等同于git@github.com:EvannaLynch/test_git_remote.git

这也可以使用`git remote -v`来查看
test    git@github.com:EvannaLynch/test_git_remote.git (fetch)
test    git@github.com:EvannaLynch/test_git_remote.git (push)

若不加-v，则只显示当前存在的shortname，不显示其代表的远程仓库具体地址
test

可以使用`git remote add`添加新的shortname，使用`git remote remove`删除已存在的shortname

在本地新建一个仓库之后，想把远程仓库同步过来，可以按以下步骤操作：
```
git init
git remote add shortname url
git fetch shortname
git merge shortname/master
```
在`git merge`之前还可以使用`git diff`功能来对比本地与远程分支的差异。

`git fetch`+`git merge`=`git pull`，但`pull`会直接合并，如果有必要，还是查看一下差异再合并为好。
