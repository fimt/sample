# Branching

## Quick Legend

|Instance|Branch|Description, Instructions, Notes|
|---|---|---|
|Stable/Production|_**stable**_|Accepts merges from Working and Hotfixes|
|Working/Development|_**master**_|Accepts merges from Features/Issues and Hotfixes|
|Features/Issues|_**feature/topic-***_ (功能编号)or _**issue/topic-***_(修复bug编号)|Always branch off HEAD of _**master**_| 
|Hotfix|_**hotfix/topic-***_|Always branch off _**stable**_|


## Main Branches

The main repository will always hold two evergreen branches:

* `master`
* `stable`


# 开始

## 处理问题

### 步骤1
切换到主分支
```
$ git checkout master
```

### 步骤2
更新资料库信息
```
$ git fetch --all
```

### 步骤3
创建一个新分支并切换到该分支。（* 是该问题的号码如 #15 那就填15）
```
$ git checkout -b "feature/topic-*"
```

## 完成工作

### 步骤1
更新资料库信息
```
$ git fetch --all
```

### 步骤2
Rebase当前分支
```
$ git rebase origin/master feature/topic-demo
```

### 步骤3
通过github desktop 来发布（Publish）或推送（Push）更改过的分支


## 结案

### 步骤1
到Github.com并导航到您各自的项目 例: https://github.com/fimt/sample

### 步骤2
转到分支机构列表 e.g https://github.com/fimt/sample/branches 并点击 "New pull request" 来完成

### 步骤3
当请求pull request时，标题必须是一下关键字:

* close
* closes
* closed
* fix
* fixes
* fixed
* resolve
* resolves
* resolved

|Syntax|Example|
|---|---|
|KEYWORD #ISSUE-NUMBER|Closes #10|
|Multiple issues|Resolves #10, resolves #123|
