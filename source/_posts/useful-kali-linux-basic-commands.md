---
title: Useful Kali Linux basic commands
date: 2020-04-02T12:24:18.000Z
updated: 2020-04-02T12:24:18.000Z
category:
  - Security & Hacking
comments: true
---
**Useful Kali Linux basic commands**

In this article I will share some basic and useful commands that you can use in the terminal.

<p align="center">
  <img width="920" height="600" src="/images/kali-linux.jpg">
</p>

****free****
Provides information about available RAM and total available and available physical space and buffer exchange memory used by Kernal.
```
root@kali:~# free
```

****vi****	
Editor which used to edit the file.
```
root@kali:~# vi [file-to-open-editor]
```

****sort****	
Arranges the contents of a text file line by line.
```
root@kali:~# cat a.txt b.txt c.txt | sort
a.txt
b.txt
c.txt
```

****more****	
One screen at a time is used to display the output in the terminal.
```
root@kali:~# more a.txt
```

****less****	
Used to view the file instead of opening the file. It does not open the entire file at once. Used for big files.
```
root@kali:~# less huge.txt
```

****date****	
This command is used to display the system date and time.
```
root@kali:~# date
```

To change the date
```
root@kali:~# date --set=’4 Jan 2019 11:20′
```

****cal****	
Shows the formatted calendar from the current month.
```
root@kali:~# cal
```

****whoami****	
Prints the active ID of the user. Also, ****who**** command prints the information about the user that is currently logged in.
```
root@kali:~# whoami
root
root@kali:~# who
root     :1             2019-01-04 11:20 (:1)
```

****pwd****	
Abbreviation for "Print Working Directory", which prints the name of the directory in operation.
```
root@kali:~# pwd
/root
root@kali:~# cd /root/Desktop/myApp/
root@kali:~/Desktop/myApp# pwd
/root/Desktop/myApp
root@kali:~/Desktop/myApp#
```

****ls****	
This command is used to show all files.
```
root@kali:~# ls
a.txt    b.txt    c.txt    worksplace
```

****users****	
Displays the login names of recently logged in users.
```
root@kali:~# users
root
```

****uptime****	
Indicates when the system is on and active users.
```
root@kali:~# uptime
15:17:10 up 20 min, 1 user, load average: 0.11, 0.19, 0.20
```

****uname****	
Prints information about the current system.
```
root@kali:~# uname
```

Also, use --help to read more about this command.
```
root@kali:~# uname --help
```
****rm****	
rm(remove) is used to delete files and directories.
```
root@kali:~# rm           # Delete files.
root@kali:~# rm -f        # Delete read only files.
root@kali:~# rm -r        # Delete the folders.
root@kali:~# rm - rf *    # Delete everything in current folder.
root@kali:~# rm - rf .    # Delete current folder with its subfolders.
root@kali:~# rm - rf /    # Delete everything in root.
```

****mv****	
This command moves or renames files and directories in the file system.
```
root@kali:~# mv [options] source dest
```

Move a.txt b.txt to /home/usr/myFiles/
```
root@kali:~# mv a.txt b.txt /home/usr/myFiles/
```

****history****	
This command is used to print the current user bash history.
```
root@kali:~# history
```
Or you can save the history in txt file for example:
```
root@kali:~# history > myHistory.txt
```
myHistory.txt will be created.

****cat****	
cat is a standard Unix utility that reads files sequentially, writing them to standard output. The name is derived from its function to concatenate files.
```
root@kali:~# echo "I am learning Linux commands" > sample.txt
root@kali:~# cat sample.txt
I am learning Linux commands
root@kali:~#
```

****mkdir****	
Used to create directories.
```
root@kali:~# mkdir [your-new-directory-name]
```

****cd****	
Used to change or switch a currently working .
```
root@kali:~# cd [your-directory-name]
```

****cp****
Used to copy.
```
root@kali:~# cp sample.txt /root/Desktop/sample.txt
root@kali:~# ls /root/Desktop/
sample.txt
root@kali:~#
```