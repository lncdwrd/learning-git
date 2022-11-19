### Compare Files
`diff -u file-1.js file-2.js`

### Generate Diff File
`diff -u file-1.js file-2.js > changes.diff`

### Apply Changes
`patch file-1.js < changes.diff`

# Git

### Initialize Git repository
`git init`

### Add files to staging area
`git add .`

### Check status
`git status`

### Log the commits
`git log`, `git log --oneline`, or `git show hash-id`

### Delete
`git rm`

### Rename
`git mv file-1.js new-file-name.js`

### Undo before staging
`git restore file-1.js`

### Remove file from staging
`git restore --staged file-1.js`

### Amend commit
`git commit --amend`

### Rollback
`git revert hash-id`

### Create new branch
`git branch new-branch-name`

### List local branches
`git branch`

### List remote branches
`git branch -r`

### Navigate branch
`git checkout branch-name`

### Create and switch
`git checkout -b new-branch-name`

### Delete branch
`git branch -d branch-name`

### Check for remote changes
`git remote show origin`

### Fetch new data
`git fetch`

### Log commits after fetch
`git log origin/main`

### Merge commits
`git merge origin/main`

### Sync and Merge
`git pull`

### Fetch all branches
`git remote update`

### Rebase
`git rebase -i HEAD~2`

### Updating Origin via Token
`git remote remove origin`
`git remote add origin https://<TOKEN>@github.com/<USERNAME>/<REPO>.git`
`git remote -v`

# Scenarios

### Uncommitted changes, Need to fetch and merge
```
git stash -u
git stash list
git fetch
git checkout origin/main
git branch main
git merge origin/main
git stash apply 0
```
