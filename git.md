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

## Remote control | Connect your local repo to remote (per project)

- `git remote add origin <urlfromgithub>`
   - Add a remote
- `git remote add set-url origin <urlfromgithub>`
   - Set a remote
- `git push origin master`
- `git remote -v`
   - View remote
- `git pull origin <urlfromgithub>`
    - Pull changes from remote

## Fork and Clones

- ...

## Checkout branch

- `git checkout -b <branch-name>`
