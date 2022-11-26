# Git Tutorial

## Introduction

Git is a very popular system of version control. The more details you can find out at [git official site](https://git-scm.com/book/en/v2)

## Repository initialization command

Use the command below to create repository in the folder.

```
git init
```

## Command to view status of the repository

Use the command below to check repository status, which files files staged or not.

```
git status
```

## Command to add file for staging and commit

Use the command below to add file to the staging or for commit.

```
git add
```

## Command to commit

Use the command below to commit changes

```
git commit -m "description"
```

## Command to view all commits

Use the command below to view all commits in the branch into repository. Use q to exit from the command.

```
git log
```

The commit log example ![Git log screenshot](GitLog.jpg) it shows all commits with their hash-codes, author and time.

## Command to switch to the commit

Use the command below to switch to a commit via hex code. It is accepted to use only 4 first symbols.

```
git checkout hex-code
```

 Use the commad with master value to switch to the actual version.

```
git checkout master
```

## Command to compare files difference

Use the command below to show the difference the between current file version and commited.

```
git diff
```

## Command to change comment for the last commit

Use the command below to change the comment in the last commit.

```
git commit --amend -m "text"
```

### Example:

__*Initial commit:*__

commit ea86d875558091dfe24abc6145899a2013b6cdd3 (HEAD -> master)
Author: Vadim Yukin <yvadim@mail.ru>
Date:   Mon Nov 21 15:52:07 2022 +0300
docs: add comment changes in the last commit

__*The last commit's comment correction command:*__

yukin@notebook-yukin MINGW64 /c/Seminar1 (master)
$ git commit --amend -m "docs: add how to change comment in the last commit"
[master 72a5d1f] docs: add how to change comment in the last commit
 Date: Mon Nov 21 15:52:07 2022 +0300
 1 file changed, 8 insertions(+)

__*git log results after that*__

$ git log
commit 72a5d1f426df0ad17a6766bfe4277b741dc55b25 (HEAD -> master)
Author: Vadim Yukin <yvadim@mail.ru>
Date:   Mon Nov 21 15:52:07 2022 +0300

docs: add how to change comment in the last commit

## Command to create a new branch

Use the command below to create a new branch.

```
git branch branch_name
```

## Command to merge branches

Use the command below to merge **current branch** with entered.

```
git merge branch_name
```

## Command to delete branch

Use the command below to delete branch.

```
git -d branch branch_names
```

## Command to clear terminal command history

Use the command below to to clear terminal command history.

```
clear
```

## Command to change directory

Use the command below to to change directory

```
cd path
```

__*Example*__

```
cd /c/Lessons/
```
## Command to create directory

Use the command below to to create directory

```
mkdir folder_name
```

## Command to create file

Use the command below to to create file

```
touch filename
```

## Command to output file content to the console

Use the command below to output file content to the console

```
cat file_name
```

## Command to append text to the end of file

Use the command below to append text to the end of file

```
echo "text to add">>file_name
```

## Command to view command history

Use the command below to view command history

```
history
```

## Command to view current directory list

Use the command below to view directory list

```
ls -l
```