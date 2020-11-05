# test_git_remote
To test the configuration

I'm learning how to use a remote git repository.

This file is created on-line then modified locally.

使用
git remote add shorname url
创建一个短名，来代替远程仓库的名称（网址、用户名、仓库名）

例如
git remote add test git@github.com:EvannaLynch/test_git_remote.git
则以后test等同于git@github.com:EvannaLynch/test_git_remote.git

这也可以使用git remote -v来查看
test    git@github.com:EvannaLynch/test_git_remote.git (fetch)
test    git@github.com:EvannaLynch/test_git_remote.git (push)

若不加-v，则只显示当前存在的shortname，不显示其代表的远程仓库具体地址
test

可以使用git remote add添加新的shortname，使用git remote remove删除已存在的shortname