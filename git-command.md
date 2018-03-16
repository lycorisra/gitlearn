## git常用命令

### 文件对比
```git diff [file]```
### 查看日志

- 查看日志
```git log [filename]```
- 查看日志 - 带参数
```git log --pretty=oneline```

### 版本回退
使用```git reset --hard [commitid]```
在git中，用```HEAD```表示当前版本，上一个版本就是```HEAD^```，上上一个版本就是```HEAD^^```，往上100个版本就是```HEAD~100```
```git reset --hard HEAD^```
- 使用```git reflog```获取操作日志引用
- 撤销暂存区的修改：```git reset HEAD [file]```

### 管理修改
git为什么比其他版本控制系统设计得更优秀，是因为Git跟踪并管理得是修改，而非文件
- 撤销修改
```git checkout -- [filename]```或者```git reset HEAD [file]```
小结
又到了小结时间。

场景1：当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用命令git checkout -- file。

场景2：当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步，第一步用命令git reset HEAD [file]，就回到了场景1，第二步按场景1操作。

场景3：已经提交了不合适的修改到版本库时，想要撤销本次提交，参考版本回退一节，不过前提是没有推送到远程库。

### 查看文件内容
```cat git-command.md```

### 删除文件
```rm [file]```



