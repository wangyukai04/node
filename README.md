## git

- 分布式 可以管理代码,合并代码
- svn集中式 速度慢, 不容易备份

## mac下

- 增强mac下的命令窗口 oh-my-zsh iterm2

## cd changeDirectory

## 告诉git你是谁(否则无法提交)

- 查看当前git配置列表
```
git config --list

fit config --global user.name
fit config --global user.email
```

## 删除文件夹

rm -rf .git

## 管理文件

- 初始化git, 告诉git哪个文件夹归你管理
```
mkdir git-repo   //创建目录

ls-a

touch index.txt   //创建空文件

```

> git仓库不能嵌套

## touch 创建文件

可以创建以点开头的文件

## cat 查看文件

## vi

- i 插入
- ESC :wq! 保存退出

## 增加暂存区

`git add ./-A`

> 在工作区中的文件是红色的, 添加到暂存区是绿色的

## 添加到历史区

`git commit -m 'xxx'`

## 查看状态

`git status`

## 查看提交日志

`git log`

## 移除本次的add

`git reset HEAD 文件名`

## 从暂存区中覆盖掉工作区

`git checkout 文件名`

## 回滚

- 将工作区 暂存区 历史区用同一个版本全部覆盖掉

  `git reset --HARD 版本号`
  
## 分支管理

- 查看分支 `git branch`

- 创建分支 `git branch dev`

- 切换分支 `git checkout dev`

> 创建并切换 `git checkout -b dev`

> 只有将内容提交到某个分支上, 这个内容才会归属于那个分支, 别的分支就看不到内容了

## 合并分支

`git merge dev`

## 提交

第一次提交不能使用这个命令
`git commit -a -m"xxx"`

> 产生冲突需要手动解决冲突  删掉不需要的内容, 提交最终的结果

> rebase cherry-pick

## 提交到远程仓库

- git init
- touch .gitignore 写上忽略的内容
- 创建需要提交的文件(空文件夹不会被提交)
- 添加到暂存区
- 添加到历史区

> 保证github是可用状态

## 链接远程仓库

git remote add origin(别名) 地址

git remote -v // 查看关联的仓库

git remote rm 别名 //可删除链接

## 推送

git push origin master


test
