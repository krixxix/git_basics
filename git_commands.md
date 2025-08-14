# Seznam klíčových příkazů
Všechny příkazy začínají klíčovým slovem **git**.

## Obecné 
|cmd příkaz|popis|
|-|-|
|``git status``|zobrazí status repozitáře|
|``git add + filename.extension`` | Přidá <filename.extension> do staging area (u souboru chci sledovat změny)|
|``git add .``|přidá celý obsah repozitáře do staging are (kromě obsahu souboru .gitignore)|
|``git commit -m "message"`` | vytvoří commit + název commitu|
|``git commit`` |taky lze, ale otevře VIM v CMD: (ESC, ``:wq`` = save & quit)|
|``git clone + https link`` |Klonuji GitLab repozitář do lokálu|
|``git push``| pushuji lokální repozitář do GitLabu|
|``git pull``|stahuji up-to-date verzi repozitáře z GitLabu|
|``git log --oneline``|zobrazí lokální historii commitů|
|``git diff``|...|
|...|...|

## Další příkazy:

### Commit reset
|cmd příkaz|popis|
|-|-|
|``git reset`` | reset the "git add" command|
|``git reset --hard``|reset to the last commit (discard current changes)|
|``git reset --hard <commit_hash>``|reset to the specified commit (all subsequent commits will be discarded)|
|...|...|


### User settings
|cmd příkaz|popis|
|-|-|
|``git config --global user.name "user_name"``| set global user name|
|``git config --global user.email "user_email"``| set global user email|
|``git config --global --list``|check global settings|
|``git config user.name "user_name"``|set local user name -> **!nutno stát ve vybraném repo!**|
|``git config user.email "user_email"``|set local user email -> **!nutno stát ve vybraném repo!**|
|``git config --list``|check local user settings|
|...|...|

## Branches
|cmd příkaz|popis|
|-|-|
|``git branch``||
|``git checkout``||
|...|...|

## Repos etc.
|cmd příkaz|popis|
|-|-|
|``git remote -v``| list remote repos|
|``git remote set-url origin <link>`` | change remote repo|
|``git remote add <name> <link>``|add new repo as a new remote|
|...|...|
