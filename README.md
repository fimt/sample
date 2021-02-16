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