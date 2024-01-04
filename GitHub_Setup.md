# Git Tutorial 

## Configuring Git

- git config --global user.name "github_username"
- git config --global user.email "github_emailid"
- git config --list

## Clone & Status

Clone - Cloning a repository on our local machine
- git clone <-repo_link->

Status - displays the state of the code
- git status

```sh 
Notes:-
  untracked- new files that git doesnt yet track
  modified- changed
  staged- file is ready to be committed
  unmodified- unchanged
```

## Add & Commit

add - adds new or changed files in your working directory to the Git staging area.
- git add <-file name->

commit - it is the record of change
- git commit -m "some message"

## Push Command

push - upload local repo content to remote repo
- git push origin main

```sh
origin - name of our repo
main - push to main branch
```

## Init Command

init - used to create new git repo

- git init
- git remote add origin <-repo_link->
- git remote -v (to verify remote)
- git branch (to check branch)
- git branch -M main (to rename branch)
- git push origin main

```sh
  *git push -u origin main
-u is added to set upstream, so if we want to work for long duration of time we have to use it once, so next time we only need to write it as "git push"
```

## Git Branches

if we wont to work on same code with two or more different features we make a branch
- git branch (to check branch)
- git branch -M main (to rename branch)
- git checkout <-branch name-> (to navigate)
- git checkout -b <-branch name-> (to create new branch)
- git checkout -d <-branch name-> (to delete branch)

##Merging Code

- git diff <-branch name-> (to compare commits, branches, files & more)
- git merge <-branch name-> (to merge 2 branches)

<center>OR</center>

- Create Pull Request
 
## Pull Command

 - git pull origin main

 used to fetch and download content from a remote repo and immediately update the local repo to match that content.

## Resolving Merge Conflicts
An event that takes place when git is unable to automatically resolve differences in code between two commits.

1. PullRequest
2. Git merge

## Undoing Changes

### Case 1: staged changes

- git reset <-filename->
- git reset

### Case 2: commited changes (for one commit)
 - git log (to check all logs of commit)
 - git reset HEAD~1

### Case 3: commited changes (for many commits)

 - git reset <-commit hash->
 - git reset --hard <-commit hash->

## Fork

A fork is a new repository that shares code and visibility settings with the original "upstream" repository

> Fork is a rough copy