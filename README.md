#Linux_Fundamental
# -Learning-Linux-Fundamental

This repository tracks my learning of  Linux basics: CLI, permissions, processes, users, tar, cron.
  I learnt the basics of linux from Linuxjourney.com, then i began from the history of linux and after that, i began the understand the rules and fuction of the different types of unix linux system
  
##1 Command-Line
									NAVIGATION
command:'pwd' - Print Working Directory (It shows the current directory path you are working on)
 e.g
*** ```bash-$ pwd
   /home/harry        ***

command:'ls' - List files(list files in the directory)
e.g
*** ```bash-$  ls
   Desktop  Documents  Downloads  -Learning-Linux-Fundamental  	***
$ls -a    #list all the hidden files that start with '.'
		(e.g; .icons .themes etc)
$ls -l    #list the files in long format
	  (e.g; drwxr-xr-x  2 harry harry 4096 F-Ɛ 22 16:46
						 Desktop)
$ls -la   #With the combination of '-la'or'-al'doesn't matter it
	   list both hidden and unhidden files in long format
 
command:'cd'- Change from one directory to another
e.g
***  ```bash-$ cd Downloads
    ~/Downloads      ***       #This shows you that you are in the Downloads directory
$cd~      #go to previous directory
$cd..     #go to home directory 

										FILES
command: 'touch' - helps to create or add a new file in a directory, & can also edit or copy timestamp
e.g
*** ```bash-$  touch ~/Downloads/first.dotx      # command that creates file and file-type  
    ```bash-$  stat ~/Downloads/first.dotx     # command to checks file timestamp
            Access: 2025-10-02 14:41:34.782807037 +0000   
            Modify: 2025-10-02 14:41:34.782807037 +0000   
            Change: 2025-10-02 14:41:34.782807037 +0000   
    ```bash-$  touch -t 202705231453.45 ~/Downloads/first.dotx   # yyyymmddhhmm.ss
    ```bash-$  stat ~/Downloads/first.dotx   #  this check the edited timestamp
	          Access: 2027-05-23 14:53:45.000000000 +0000   # atime(access time)
            Modify: 2027-05-23 14:53:45.000000000 +0000   # mtime(modify time)
            Change: 2025-10-02 16:35:46.964345502 +0000   # ctime(change time)
    ```bash-$  touch ~/Downloads/second.dotx     # create a new file with the timestamp
    ```bash-$  touch -r ~/Downloads/first.dotx second.dotx #copied first timestamp to second
    ```bash-$  stat ~/Downloads/second.dotx ***     # this check the copied and edited timestamp 
    
command: 'file' - used to identify the exact filetype of a file
    ```bash-$  file ~/Downloads/first.dotx
            /home/name/Downloads/first.dotx: PDF document, version 1.7

command: 'cat' - used to to read a text file in terminal
*** ```bash-$  cat ~/Downloads/first.dotx  ***

command: 'less' - used to read and display file in page form
*** ```bash-$ less ~/Downloads/first.dotx  ***

command: 'history' - it shows last 15 command that you typed in the shell or terminal
*** ```bash-$   history         ***
       662  touch -r ~/Downloads/first.dotx
       664  stat ~/Downloads/first.dotx
       669  stat ~/Downloads/second.dotx   # and 10 more history
       670  touch ~/Downloads/first.dotx
       676  touch -t ~/Downloads/first.dotx 
*** ```bash-$ !!   ***    # use to print recent or previous command
*** ```bash-$                                                    ✔ 
          bck-i-search: _          # when u use "CTRL+C" the u can search for your previous command
*** ```bash-$ clear  ***          # this is used to clean or restart the terminal


## Day 2: Permissions
...

## Day 3: Processes
...

## Day 4: Users & Groups
...

## Day 5: tar Backups
...

## Day 6: Cron Jobs
...

## Day 7: Review