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

## Revert a folder to a previous commit

`git rm -r /path/to/dir`

`git checkout <rev> /path/to/dir`

`git commit -m "reverting directory"`

## Check the alias / address of Git Remote

`git remote -v`

## view last commit details

`git log -1`

## Add new changes to previous commit

1. `git add <files>`
2. `git commit --amend --no-edit`

## Amend the commit message of previous commit

`git commit --amend`

## Create a new branch

`git checkout -b <newBranchName>`

## Rename a branch

`git checkout oldBranchName`

`git branch -m newBranchName`

## Switch to another branch

`git checkout <branchName>`

## Move to previous branch

`git checkout -`

## Delete a branch at local

`git branch -d <branchName>`

## Delete remote branch

`git push origin --delete <branchName>`

## How to bring a remote branch to local 

`git checkout <feature/CPDT-18416>`

`git pull

## Write a Git command on multiple lines

`git add firstFile.txt \`

`secondfile.txt`

## Know your git version

`git --version`

## Merge Master branch to your branch

`git checkout <featurebranch>` go to your feature branch

commit if any changes are there

`git rebase <master>`

## Get out of 'detached head state'

`git checkout -`

Note: you lose all the commits made in detached head state

## Diff when you have not 'git add' any files yet

`git diff`

## Diff with last commit

`git diff --cached`

## Combine of `git diff` and `git diff --cached`

`git diff HEAD`

## Diff between current state and a certain commit

`git diff <commit hash>`

## Stash the changes

`git stash`

## Restore the Stash

`git stash apply`

## Undo the last commit, while leaving your working tree untouched

`git reset HEAD~`

## Configure the default diff tool

`git config --global diff.tool kdiff3`

## View the files between two commits in the default difftool

`git difftool Head~33..Head`

## Squash the commits

1. git checkout master
2. git pull
3. git checkout -b <new branch>(new branch with one commit for all the commits)
4. git checkout <your branch>(the branch to squash)
5. git push(create backup)
6. git checkout <new branch>
7. git merge --squash <your branch>
8. git commit -m "message for the single squashed commit"
9. git log --oneline --graph

## Difference between local branch and origin

`git difftool origin/branchname`



## Check the url of remote

`git remote show origin`



### Remove untracked files

`git clean -n` (dry run)

`git clan -f`(actual command)

















git 
