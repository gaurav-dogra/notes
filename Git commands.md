# Git commands

## Push your current Project to Github

1. `Git init`
2. Add .gitignore
3. Commit the code
4. Create a repository on Github
5. `git remote add origin https://github.com/gaurav-dogra/InspectionAPI.git`
6. git push origin main

# Commit

### Picking parts from a single file to add to a commit

 `git add -p <fileName>`

### Writing a commit message with a body

`git add <file/s>` 

`git commit (opens editor window)`

`<first line is subject>`

`<empty line>`

`<commit body>`

### Adding only tracked files for next commit

`git add -u`

### Adding only untracked files for next commit

`git add -i (4) (*) (q)`

### Revert a file to previous commit

`git checkout <filename>`

### Revert/reset a file to another branch

`git checkout <branchname of desired file> -- <file path>`

### Revert all local un-staged changes

`git checkout .`

### Revert all staged and un-staged changes

`git reset HEAD`

`git checkout .`

### Revert a folder to a previous commit

`git rm -r /path/to/dir`

`git checkout <rev> /path/to/dir`

`git commit -m "reverting directory"`

### view last commit details

`git log -1`

### Add new changes to previous commit

1. `git add <files>`
2. `git commit --amend --no-edit`

### Amend the commit message of previous commit

`git commit --amend` and press enter

### How to reset last commit on local

git reset --soft HEAD~1

===================================================================================================



## List all the files that are being tracked

git ls-tree -r master --name-only

## Remove a folder from git tracking

- Add <folderpath> to gitignore 
- `git rm -r --cached <folderpath>`

## Check the alias / address of Git Remote

`git remote -v`

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

`git pull`

## Write a Git command on multiple lines

`git add firstFile.txt \`

`secondfile.txt`

## Know your git version

`git --version`

## Merge Master branch to your branch

`git checkout <featurebranch>` go to your feature branch

commit if any changes are there

`git rebase <master>`



### Abort/Cancel Merging

`git merge --abort`

## How to overwrite local branch from remote

`git fetch --all`

`git reset --hard origin/branchName`

## How to overwrite local branch with local master

git reset --hard master

## Get out of 'detached head state'

`git checkout -`

Note: you lose all the commits made in detached head state

## Diff when you have not 'git add' any files yet

`git diff`

## Diff with last commit

`git diff --cached`

## Combine of `git diff` and `git diff --cached`

`git diff HEAD`

## compare current state and a certain commit

`git diff <commit hash>`

## Stash the changes

`git stash`

## Restore the Stash

`git stash apply`

## Undo the last commit, while leaving your working tree untouched

`git reset HEAD~`

## Configure the default diff tool

`git config --global diff.tool kdiff3`

## View the files between two commits in the difftool

`git difftool commit~..commit`

## View the changes brought in by a commit

`git diff commit~ commit`

## View the changed files since last commit

`git diff --name-only HEAD HEAD~1`

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

## Compare two branches

`git [difftool | diff] origin/branchname`

`git [diff | difftool] master...`

## Compare Two commits GUI

`gitk firstCommit..secondCommit`

## Find what file changed in a commit 

`git log --raw`

## Check the url of remote

`git remote show origin`

### Delete/Remove untracked files

`git clean -n` (dry run)

`git clean -f`(actual command)

`git clean -f -d` (clean directories)

## Preview git pull

1. `git fetch`
2. `git log HEAD..origin/master`
