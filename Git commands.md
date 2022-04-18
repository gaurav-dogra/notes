# Git commands

## Push your current Project to Github

1. `Git init`
2. Add .gitignore
3. Commit the code
4. Create a repository on Github
5. `git remote add origin https://github.com/gaurav-dogra/InspectionAPI.git`
6.  git push origin main

## Adding only tracked files for next commit

`git add -u`

## Adding only untracked files for next commit

`git add -i (4) (*) (q)`

## Revert a file to previous commit

`git checkout <filename>`

## Revert all local uncommitted changes

`git checkout .`

## Check the alias / address of Git Remote

`git remote -v`

## Add new changes to previous commit

1. `git add <files>`
2. `git commit --amend --no-edit`

## Create a new branch

`git checkout -b <newBranchName>`

## Rename a branch

`git checkout oldBranchName`

`git branch -m newBranchName`

## Switch to another branch

`git checkout <branchName>`

## Track your remote branches explicitly 

`git branch -f <remote_branch_name> origin/remote_branch_name`

`git checkout remote_branch_name(this is local operation)`

## Write a Git command on multiple lines

`git add firstFile.txt \`

`secondfile.txt`

## Know your git version

`git --version`





