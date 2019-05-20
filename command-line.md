# Command Line

- Options modify the behavior of commands
   - `ls -a` lists all contents of a directory, including hidden files and directories
   - `ls -l` lists all contents in long format
   - `ls -t` orders files and directories by the time they were last modified
   - Multiple options can be used together, like `ls -alt`

- From the command line, you can also copy, move, and remove files and directories:
   - `cp` copies files
   - `mv` moves and renames files
   - `rm` removes files
   - `rm -r` removes directories

- `nano ~/.bash_profile`
    - Ctrl+O / Enter / Ctrl+x
- `source~/.bash_profile`
   - renders script

Example of .bash_profile
````
export PS1="\[\033[0;36m\]\u@\w\[\033[m\]\$ "
#export PS1="\u@\w$ "

export CLICOLOR=1;
export LSCOLORS=dxfxcxdxbxegedabagacad;

alias hy="history"
alias cl="clear"
alias ll="ls -la"
alias pd="pwd"

alias migrate-undo="sequelize db:migrate:undo:all && sequelize db:migrate:undo:all --env test"
alias migrate="sequelize db:migrate && sequelize db:migrate --env test"
````


