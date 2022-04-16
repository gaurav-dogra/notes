# Git commands

## How to push your current Project to Github

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

## How to check the alias / address of Git Remote

`git remote -v`

## How to add new changes to previous commit

1. `git add <files>`
2. `git commit --amend --no-edit`

## How to create a new branch

`git checkout -b <newBranchName>`

## How to switch branch

`git checkout <branchName>`

## How to track your remote branches explicitly 

`git branch -f <remote_branch_name> origin/remote_branch_name`

`git checkout remote_branch_name(this is local operation)`

## How to write a Git command on multiple lines

`git add firstFile.txt \`

`secondfile.txt`



