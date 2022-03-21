# Git commands

## Adding only tracked files to index with and ignoring untracked files for next commit

git add -u

## How to check the alias / address of Git Remote

git remote -v

## How to add new changes to previous commit

1. git add <files>
2. git commit --amend --no-edit

## How to create a new branch

git checkout -b <newBranchName>

## How to switch branch

git checkout <branchName>

## How to track your remote branches explicitly 

git branch -f <remote_branch_name> origin/remote_branch_name

git checkout remote_branch_name(this is local operation)
