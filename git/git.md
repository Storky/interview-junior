# Git

## 1. Git common commands
#### Save
`git add .` - Add files to staging

`git commit -m "Commit message"` - commit added files

`git push origin master` - Send changes to the master branch of your remote repository 

`git status` - list of changed and staged files

`git remote add origin <server>` - connect to remote repository

`git remote -v` - list of configured remote repos

`git checkout -b <branchname>` or `git branch` - list of branches in repo

`git branch -d <branchname>` - delete branch

`git push origin <branchname>` - send branch to repo

`git push origin :<branchname>` - delete branch on remote repo


## 2. Cherry Pick
Cherry Pick - https://www.youtube.com/watch?v=FdZecVxzJbk&ab_channel=CoreySchafer
1. git log to copy commits hash
2. checkout to consumer branch
3. git cherry-pick <hash .1>

#### In other words:
`git cherry-pick <commit id or ids>` - get commit from those branch to current
then commit it
`git cherry-pick <commit id or ids> -n` - -n is no commit, its like merge in


## 3. Fetch merge flow
## 4. Undo flow, hard and soft
Then, to delete src commit there are 3 types of resets - soft, hard and mixed(default)
- checkout to src branch and copy by git log next commit's hash, by cherry picked
- git reset --soft <hash .4> - it will delete commit but save changes in pre staged  folder
- git reset <hash .4> - changes will be in staged area
- git reset --hard <hash .4> - get rid of changes from followed commit
- git clean -df - get rid from changes ?? in untracked files and folders

If we want to revert unrevertable (in term of like 30 days possible)
- git reflog - history of changes and deletions
- git checkout <hash .9> - recall the changes from lost commit
- git checkout backup_branch - save it to new branch

If ppl pulled wrong changes, must to creat revert commit:
- git revert <hash of unwanted commit>
- git diff <hash1> <hash2> - shows the diff between 2 commits


## 5. Init flow
https://docs.github.com/en/github/importing-your-projects-to-github/importing-source-code-to-github/adding-an-existing-project-to-github-using-the-command-line

## 6. Rebase

OTW


## 7. Stash
https://www.atlassian.com/git/tutorials/saving-changes/git-stash

git stash
git stash pop
git stash save "add style to our site"
git stash list
