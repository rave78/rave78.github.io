---
layout: post
title:  "Useful commands for new Ph.D. students"
date:   2014-09-15 14:00:00
categories: linux
tags: noteToMyself
---
There are several tools in Linux that are really useful for any new Ph.D.
student.  

a) **Remote copy**: There cases a file (or directory) needs to be transfer from
one computer to another computer via network

scp file.h5 *#username*@*#computer*:*#location*

scp -r *#source\_directory* *#username*@*#computer*:*#location*

b) **Screen command**:  Launch any script and keep it
running in the background.  Useful if you need to review the status of your
script in a different locations

screen  --> new screen-terminal

\<Ctrl-A\> + d --> detach current screen-terminal

screen -r *#name\_screen* --> reattach to name\_screen

screen -ls --> list all screen-terminals

c) **Subsitute information in text files**

sed -i 's/*#search\_pattern*/*#substitution*' *#input\_file*

d) **Remote mounting**

sshfs *#username*@*#computer*:*#remote\_folder*
