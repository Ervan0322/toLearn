## 创建版本库

第一步创建一个空文件夹：

```bash
mkdir learngit
cd learngit
pwd
```
第二步，通过`git init`命令把这个目录变成Git可以管理的仓库
```
git init
```
> 这时，当前文件夹下会多出一个.git的目录
> 这个目录时Git来跟踪管理版本库的

## 将文件放入git仓库

1. `git add`命令，将文件放入暂存区
2. `git commit`命令，将文件放入本地仓库

```
git add readme.txt
```

```
git commit -m "xxx" [文件名]
```

为什么Git添加文件需要add，commit一共两步呢？因为commit可以一次提交很多文件，所以你可以多次add不同的文件，比如：

```
git add file1.txt
git add file2.txt file3.txt
git commit -m "add 3 files."
```

## 常用命令

* `git status`命令可以让我们时刻掌握仓库当前的状态

* `git diff`顾名思义就是查看difference，显示的格式正是Unix通用的diff格式,即比较文件的不同。

* `git log` 查看版本控制系统的历史纪录。显示从最近到最远的**提交日志**。如果嫌输出信息太多，看得眼花缭乱的，可以试试加上`--pretty=oneline`参数

* `git reset` 命令是移动版本，可以向前也可向后，主要通过移动HEAD指针来控制

> 参数：`--hard` 

* `git reflog`查看**命令历史**,以便确定要回到未来的哪个版本

[更多命令](https://www.liaoxuefeng.com/wiki/896043488029600/900002180232448)

