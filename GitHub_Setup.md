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