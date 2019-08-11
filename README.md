# linux\_home\_config

## Introduction

This is the repo to hold my HOME directory configurations in Linux.  
The main purpose of the repo is to backup and transfer settings between machines.

## Prerequisites

1. Linux
2. GNU Bash
3. vim
4. xsel (For tmux-yank plugin)

A static build of tmux 2.6 has been bundled in this repo.

## Usage

```
cd   # cd into the HOME directory
git init
git remote add origin https://github.com/hehaoqian/linux_home_config.git
git fetch origin
git checkout -b master --track origin/master

# Do this if the following path is not already in your PATH
# Add to ~/.bashrc to make it permanent
export PATH=~/.local/bin:$PATH

hash -r   # To Update bash PATH cache

tmux
# Enter "C-g, I" to install tmux plugins
```

## Update this repo

1. Because HOME directory has lots of other stuffs.  
To prevent accidentally add stuffs into this repo, .gitignore contains \* at  
the very first line. Add the path needs to be include explicitly to .gitignore

## License

This repository contains lots of third party codes.  
Including but not limited to:  
Tmux plugins: https://github.com/tmux-plugins  
Vim plugins: https://github.com/tpope  
All third party codes are licensed under their original licenses.  
Go to their official website for more information, and to get the newest versions.    
The code written by myself in this repository, such as the configuration files,  
are placed under the Public Domain.
