# Seznam klíčových příkazů
Všechny příkazy začínají klíčovým slovem **git**.

## Obecné 
|cmd příkaz|popis|
|-|-|
|``git status``|display the current local repo status|
|``git add <filename.extension>`` | add <filename.extension> into the staging area (track changes)|
|``git add .``|add everything into the staging area (except of .gitignore)|
|``git commit -m <message>`` | create commit + commit message|
|``git commit`` | also possible, opens VIM: (``ESC``, ``:wq`` = save & quit)|
|``git clone <https link>`` |clone remote repo via HTTPS|
|``git push``| push the <b>current</b> branch into remote repo|
|``git push <origin> <main>``|push the <b>main</b> branch into the <b>origin</b> remote|
|``git fetch``|download the latest changes from <b>all remote branches</b> without merging them|
|``git fetch <origin> <main>``|download content of <b>main</b> branch from <b>origin</b> remote |
|``git pull``| download and merge all changes of the <b>current</b> branch and merge them|
|``git pull origin main``|downlaod and merge changes from <b>origin</b> remote of <b>main</b> branch|
|``git log``|display commit hisotry|
|``git log --oneline``|display <b>simplified</b> commit history|
|``git diff``|shows changes in your working directory that are not staged|
|``git diff --staged``|shows changes between the staged files and the last commit|
|``git diff <commit1> <commit2>``|shows differences between two commits|
|...|...|

## Commit reset
|cmd příkaz|popis|
|-|-|
|``git reset`` | reset the "git add" command|
|``git reset --hard``|reset to the last commit (discard current changes)|
|``git reset --hard <commit_hash>``|reset to the specified commit (all subsequent commits will be discarded)|
|...|...|


## User settings
|cmd příkaz|popis|
|-|-|
|``git config --list``|check local user settings|
|``git config --global user.name "user_name"``| set global user name|
|``git config --global user.email "user_email"``| set global user email|
|``git config --global --list``|check global settings|
|``git config user.name "user_name"``|set local user name -> **!nutno stát ve vybraném repo!**|
|``git config user.email "user_email"``|set local user email -> **!nutno stát ve vybraném repo!**|
|...|...|

## Branches
|cmd příkaz|popis|
|-|-|
|``git branch``| list branches|
|``git branch -a``| list all branches (including remote)|
|``git branch <branch-name>``|create branch|
|``git checkout <branch-name>``|(<b>obsolete</b>) switch to another branch|
|``git switch <branch-name>``|switch to another branch|
|``git checkout -b <branch-name>``|create and switch to a new branch (shortcut)|
|``git remote prune <origin>``|when you delete a branch on remote ...|
|...|...|

## Pull requests
|cmd příkaz|popis|
|-|-|
|``git fetch origin pull/ID/head:pr-branch``|e.g. pr-1 for the first pr|

## Remote
|cmd příkaz|popis|
|-|-|
|``git remote -v``| list remote repos|
|``git remote set-url origin <link>`` | change remote repo|
|``git remote add <name> <link>``|add new repo as a new remote|
|...|...|
