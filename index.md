# GIT tutorial

This is our source control guide


## Repository initialization

To initialize repository (space for file source control) use next command: 

```
git init
```

## Adding files to repository

To add a file to repository use next command:

```
git add <FILE_NAME>
```

## Checking repository status

To check repository status use next command:

```
git status
```

## Commiting repository changes

To commit new repository changes use next command (where message describes what is changed):

```
git commit -m "<message>"
```

## Reviewing repository log

To track log of recent repository actions use next command:

```
git log
```

## Switching between commits

To switch between different repository commits use next command:

```
git checkout <fist four letters of commit name>
```

## Returning to current (master) commit

To return to master commit and continue work use next command:

```
git checkout master
```

## Comparing the difference between current and last commited version

To see the differnce between current uncommited file and it's last commited version use next command:

```
git diff
```

## Changing last commit name

To change the name of last commit use next command (where mesage is the new name of last commit):

```
git --amend commit -m "<mesage>"
```

## New folder creation

To create a new folder in selected repository use next command:

```
mkdir <FOLDER_NAME>
```

## Terminal command history

To track the history of all used commands (within terminal) use next command:

```
history
```

## New branch creation

To create a new branch use next command:

```
git branch <branch_name>
```

## Branch check

To check all existing branches and track selected one use next command:

```
git branch
```

## Merging branches

To merge selected branch with one we are trying to merge use next command:

```
git merge <branch_to_merge>
```

## Cloning remote repository URL

To clone a remote repository to local PC use next command:

```
git clone <URL_of_remote_repository_to_clone>
```

## Pulling remote repository data

To pull remote repository data and to merge it with local repository use next command:

```
git pull
```

## Pushing local data to remote repository

To push local repository data to remote one use next command:

```
git push
```

## Setting new remote URL origin

To drop previous repository link and to create a new URL link of local repository use next command:

```
git remote set -url origin <URL_adress_of_repository>
```