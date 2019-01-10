#GIT Cheatsheet

Install GIT http://git-scm.com/downloads or https://desktop.github.com/

##Check install and create user environment

- git --version
- git config --global user.name “Tai Dang”
- git config -- global user.email “tai.dangit@gmail.com”

##Create a local repo & environment

- mkdir YOUR-NEW-PROJ-FOLDER
- cd YOUR-NEW-PROJ-FOLDER
- git init

##Commit to it

- Git status
- Git add readme.txt
- Git commit -m “your note”

##Connect to GitHub

- Git config —global user.username <USERNAME>
- Git config —global user.username

##Remote control | Connect your local repo to remote (per project)

- Git remote add origin <urlfromgithub>
-- Add a remote
- Git remote add set-url origin <urlfromgithub>
-- Set a remote
- Git push origin master
- Git remote -v
-- View remote
- Git pull origin <urlfromgithub>
    - Pull changes from remote

##Fork and Clones

- ...

##Checkout branch

- Git checkout -b <branch-name>

##Workflow

- git checkout -b branch-name: Create and checkout a branch to begin working.
- git add --all: Adds all the modified and untracked files to the staging area. You can add them one at a time by using git add filename.
- git commit -m "message that tells what the commit is doing": Commits files in the staging area.
- git checkout master: Moves you back to the master branch.
- git merge branch-name: Merges the work you did in your branch into master.
- git push: Will push your work to the origin repository's master branch.
