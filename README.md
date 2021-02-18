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

Rebase your current branch
```
$ git rebase master
```