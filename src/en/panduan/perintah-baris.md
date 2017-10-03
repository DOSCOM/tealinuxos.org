---
title: Command Line
type: panduan
order: 113
---

## General Commands List ##
To explore or move on TealinuxOS or other linux distro in addition to using Graphical User Interface (GUI) you can also use Command Line Interface (CLI). The following are some commonly used commands in the CLI.

- See the directory we are on
  The `pwd` or print working directory command is used to determine the position of the directory to which we belong.
  `` `
    $ pwd
  `` `

- Move Directory

  The `cd` command is used to change the directory where we are. cd [directory_name] To return to the level one prior level command is used as follows.
  `` `
    $ cd.
  `` `
  To return to the root directory the command is as follows.
  `` `
    $ cd ..
  `` `

- List

  The `ls` command is used to display a list of files in the directory. ls To display a list of files in a particular directory
  `` `
    $ ls [directory_name]
  `` `

- Copying File
  
  The `cp` command is used to copy a file or directory to another directory.
  `` `
    $ cp [filename] [directory_name]
  `` `

- Moving Files

  The `mv` command is used to move files or directories to another directory.
  `` `
    $ mv [filename] [directory_name]
  `` `

- Deleting Files
  
  The `rm` command is used to delete files or directories to another directory.
  `` `
    $ rm [filename]
  `` `

- Commands usage
  The `man` command is used to display how to use a command.
  `` `
    $ man [name_perintah] man rm
  `` `


## Running Commands with Administrative Rights
When you work with line commands, some commands can not be performed without administrator privileges, so it takes the sudo command at the start of each command. Shortly after you give the sudo command the system will ask for a password and will remember it for 15 minutes. Within these 15 minutes you can run the sudo command without typing a password every time you run the command. `` ` 
  $ sudo apt-get update
`` `