# GIT Cheatsheet

Install GIT http://git-scm.com/downloads or https://desktop.github.com/

## GENERAL Workflow

- `git checkout -b branch-name`
   - Create and checkout a branch to begin working.
- `git add --all`
   - Adds all the modified and untracked files to the staging area. You can add them one at a time by using git add filename.
- `git commit -m "message that tells what the commit is doing"`
   - Commits files in the staging area.
- `git checkout master`
   - Moves you back to the master branch.
- `git merge branch-name`
   - Merges the work you did in your branch into master.
- `git push`
   - Will push your work to the origin repository's master branch.

## Check install and create user environment

- `git --version`
- `git config --global user.name “Tai Dang”`
- `git config -- global user.email “tai.dangit@gmail.com”`

## Create a local repo & environment

- `mkdir YOUR-NEW-PROJ-FOLDER`
- `cd YOUR-NEW-PROJ-FOLDER`
- `git init`

## Commit to it

- `git status`
- `git add readme.txt`
- `git commit -m “your note”`

## Connect to GitHub

- `git config —global user.username <USERNAME>`
- `git config —global user.username`

## General

`git status`


## Remote control | Connect your local repo to remote (per project)

`git remote add origin <urlfromgithub>` // Add a remote
`git remote add set-url origin <urlfromgithub>` // Set a remote
`git push origin master`
`git remote -v` // View remote
`git pull origin <urlfromgithub>`//  Pull changes from remote

## Fork and Clones

...

## Checkout branch

`git branch` // view local branch and to see which branch you are on
`git checkout -b <branch-name>` create new feature branch and switch over to it
`git checkout master` switch to master


## Commiting

`git commit -m 'commit message`

## Merging

Switch to a branch/master to merge another branch/master into it

`git merge name-of-branch-or-master`
`git push` pushes to master
`git push origin name-of-branch` pushes to feature branch

## Resetting branch to start clean again

`git reset --hard HEAD`
`git clean -fd`

