# Git Commands Reference
This repository serves as a guide for essential Git commands, ranging from basic setup to undoing changes.

## Clone and Status
Clone: Cloning a repository on our local machine.

```
git clone <repository-link>
```
Status: Displays the status of the code.

Untracked: New files that Git doesn't yet track.

Modified: Changed files.

Add/Staged: File is ready to commit.

Commit/Unmodified: Unchanged files.

```
git status
```

## Hidden files: To display hidden files in the terminal.
```
ls -a
```
## Add and Commit
Add: Adds new or changed files in your working directory to the Git staging area.
```
git add .
```
OR
```
git add <file-name>
```
Commit: It is the record of change.
```
git commit -m "some message"
```
## Push
Push: Upload local (laptop) repo content to remote (GitHub) repo.
```
git push origin <branch-name>
```
## Init Command
Init: Used to create a new Git repo.
```
git init
```
Remote Add: Links the local repo to the remote server.
```
git remote add origin <link>
```
Verify Remote:
```
git remote -v
```
Check Branch:
```
git branch
```
Rename Branch:
```
git branch -M main
```
# Branch Commands
List Branches:
```
git branch
```
Exit/Switch Branch:
```
git checkout <branch-name>
```
Create and Switch:
```
git checkout -b <new-branch-name>
```
Delete Branch:
```
git branch -d <branch-name>
```
## Merge Commands
## Method 1 (CLI)
Compare branches:
```
git diff <branch-name>
```
## Merge branches:
```
git merge <branch-name>
```
## Method 2
Pull Request through GitHub UI.

Pull Command
Pull: Used to fetch and download content from remote (GitHub) repo to local (laptop) repo to match the content immediately.
```
git pull origin main
```
## Undoing Changes
Case 1 (Staged Changes): If the file is not committed yet.
```
git reset <file-name>
```
Case 2 (Committed Changes): For one commit.
```
git reset HEAD~1
```
Case 3 (Multiple Commits): Reset to specific point:
```
git reset <commit-hash>
```
## Force reset (Local & Remote):
```
git reset --hard <commit-hash>
```
