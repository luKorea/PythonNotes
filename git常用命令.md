### git常用命令

##### 1.全局配置git用户名邮箱

```
  git config --global user.name '你的名字'
  git config --global user.email '你的邮箱地址'
```

##### 2. 创建本地库

```git
git init 
```

##### 3. 把本地文件（工作区）添加到缓存区

```git
git add read.txt：
```

##### 4. 把本地所以文件全部添加到缓存区

```git
git add . 
```

##### 5. 把缓存区的所有文件都添加到仓库上

```git
git commit -m 'describe message'
```

##### 6. 将本地仓库与远程仓库进行合并

```
git remote add origin "你的远程仓库地址"
```

##### 7. 推送到远程仓库

```git
git push -u origin master
```

##### 8. 查看git仓库当前的状态

```
git status
```

##### 9. 查看文件具体修改了哪里

```git
git diff read.txt
```

##### 10. 查看最近到最远提交到仓库的文件信息（一串数字为特有的时间序列id 可以根据它进行版本前后回滚）

```git
git log
```

##### 11. 回退到上一次 commit的时候

```git
git reset --hard HEAD^
```

##### 12. 版本前进 只能根据 id进行前进（id只写出前六位就好了)

```git
git reset --hard bdeacd
```

##### 13. 查看每次操作仓库内的信息（commit） 这样的话当黑窗口没了的时候，也可以查询具体操作信息，进行版本回退或者前进!

```git
git reflog
```

##### 14. 工作区恢复到最近一次的commit或者add

```git
git checkout -- read.txt
```

##### 15. 删除某一个文件

```git
git rm read.txt
```

##### 16. 创建dev分支

```git
git branch dev
```

##### 17. 切换到dev分支上开发

```git
git checkout dev
```

##### 18. 查看所有分支

```git
git branch
```

##### 19. 删除分支 （-D 强制删除）

```git
git branh -d dev
```

##### 20. 合并分支

```git
git merge dev
```

