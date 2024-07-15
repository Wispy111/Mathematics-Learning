---
date: 2024-07-14
---
```mermaid
graph LR
A["工作区"]
B["暂存区"]
C["本地仓库"]
D["远程仓库"]

A -->|"git add"| B 
B -->|"git commit"| C
C -->|"git push"| D
D --> |"git pull"| C
```

## Shell 命令
一般而言，Shell 命令有如下三个组成部分：

- 命令所需程序；
- 命令类型；
- 命令参数；

以 `git` 的命令为例：

```shell
git add .
```

这里我们调用了 `git` 程序，类型是 `add` ，参数传入的是 `.` ，参数代表的意义是当前文件夹目录.

## 更改并上传的工作流程

进入工作区先进行同步：

```shell
git pull
```

更改想要的部分之后可以 `add` ：

```shell
git add .
```

然后再进行 `commit` ：

```shell
git commit -m "The info of the repository"
```

最后上传到远程仓库：

```shell
git push
```

