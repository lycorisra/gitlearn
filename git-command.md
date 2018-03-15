## git常用命令

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


