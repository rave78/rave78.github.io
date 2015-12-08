---
layout: post
title:  "Tips for new Ph.D. students"
date:   2014-09-15 14:00:00
categories: linux
tags: noteToMyself
---
As a fomer lecturer of CS department at [ESPOL](http://www.fiec.espol.edu.ec), I am really happy that the first [Ph.D. program](http://dcca.espol.edu.ec/) was launched.  With this in mind, I want to share with the new students some tips that I found quite useful during my research. 

a) **Remote copy**: There are cases that a file (or directory) needs to be transfer from
one computer to another computer via network

    scp file.h5 *#username*@*#computer*:*#location*

    scp -r *#source\_directory* *#username*@*#computer*:*#location*

b) **Screen command**:  Launch any script and keep it running in the background.  Useful if you need to review the status of your script in a different locations

    screen  --> new screen-terminal

    \<Ctrl-A\> + d --> detach current screen-terminal

    screen -r *#name\_screen* --> reattach to name\_screen

    screen -ls --> list all screen-terminals

c) **Subsitute information in text files**

    sed -i 's/*#search\_pattern*/*#substitution*' *#input\_file*

d) **Remote mounting** 

    sshfs *#username*@*#computer*:*#remote\_folder*

e) **Join several pdf files**

    pdfunity *filename1* *filename2* ... *filenameN*

f)  **ffmpeg**: create a video from a set of images (given a pattern)
    
    ffmpeg -r 1/2 -i *pattern\_image* -r 30 output.mp4

g)  **Academic writing**: It sounds obvious but it is a complex task to put
in words.  I recommend two books: _Science Research Writing For Non-Native Speakers Of English: A Guide for Non-Native Speakers of English (Glasman-Deal)_ and _How to Write and Publish a Scientific Paper (Day and Gastel)_

