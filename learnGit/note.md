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

