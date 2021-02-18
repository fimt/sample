# Branching

## Quick Legend

|Instance|Branch|Description, Instructions, Notes|
|---|---|---|
|Stable/Production|_**stable**_|Accepts merges from Working and Hotfixes|
|Working/Development|_**master**_|Accepts merges from Features/Issues and Hotfixes|
|Features/Issues|_**feature/topic-***_ or _**issue/topic-***_|Always branch off HEAD of _**master**_|
|Hotfix|_**hotfix/topic-***_|Always branch off _**stable**_|


## Main Branches

The main repository will always hold two evergreen branches:

* `master`
* `stable`


# Getting Start

## Working with New Issue

### Step 1
Switch to master branch
```
$ git checkout master
```

### Step 2
Update repository information
```
$ git fetch --all
```

### Step 3
Create a new branch and switch over
```
$ git checkout -b "feature/topic-*"
```

## Finalizing Work

### Step 1
Update repository information
```
$ git fetch --all
```

### Step 2
Rebase your current branch
```
$ git rebase origin/master feature/topic-demo
```

### Step 3
Publish or Push all your branch changes


## Closing Issue

### Step 1
Go to Github.com and navigate to your respective project e.g https://github.com/fimt/sample

### Step 2
Go to the list of branches e.g https://github.com/fimt/sample/branches and click on the "New pull request" on your completed branch

### Step 3
The title of the pull request must consist of the following keywords:

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