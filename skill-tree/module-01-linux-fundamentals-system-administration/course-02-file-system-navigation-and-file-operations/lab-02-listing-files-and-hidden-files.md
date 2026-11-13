# Lab: Listing Files and Hidden Files

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, we will be tested on our ability to look at files in different branches 
- What problem were you tasked to solve?
  1. Get detailed "ID cards" for files (size, owner, date).
  2. See "invisible" files that are normally hidden.
  3. Look deep into sub-folders without entering them.

---

## 🛠️ Commands & Configuration Used
```shell
ls (list)
ls -l (list long format)
ls -a (list all files)
ls -R (list recursively)
ls -la (list all and long format)
```

---

## ✅ Results
- What was completed?
  We completed tasks using the following commands
  1. `ls`: "What is in here?" (Basic list)
  2. `ls -l`: "Show me the ID cards." (Long details: permissions, owners, size)
  3. `ls -a`: "Show me the hidden stuff." (All files, including dotfiles)
  4. `ls -R`: "Show me deep inside." (Recursive list)
  5. `ls -la`: Combine powers!
- What output or verification confirmed success?
```
labex:project/ $ ls
data  document.md  file1.txt  file2.txt  logs  script.py
labex:project/ $ ls -l
total 0
drwxrwxr-x 2 labex labex  6 Nov 13 17:34 data
-rw-rw-r-- 1 labex labex  0 Nov 13 17:34 document.md
-rw-rw-r-- 1 labex labex  0 Nov 13 17:34 file1.txt
-rw-rw-r-- 1 labex labex  0 Nov 13 17:34 file2.txt
drwxrwxr-x 3 labex labex 40 Nov 13 17:34 logs
-rwxr-xr-x 1 labex labex  0 Nov 13 17:34 script.py
labex:project/ $ ls -a 
.  ..  .config  .gitignore  .hidden_secret  data  document.md  file1.txt  file2.txt  logs  script.py
labex:project/ $ ls -la
total 4
drwxr-xr-x 1 labex labex  155 Nov 13 17:34 .
drwxr-x--- 1 labex labex 4096 Nov 13 17:39 ..
-rw-rw-r-- 1 labex labex    0 Nov 13 17:34 .config
-rw-rw-r-- 1 labex labex    0 Nov 13 17:34 .gitignore
-rw------- 1 labex labex    0 Nov 13 17:34 .hidden_secret
drwxrwxr-x 2 labex labex    6 Nov 13 17:34 data
-rw-rw-r-- 1 labex labex    0 Nov 13 17:34 document.md
-rw-rw-r-- 1 labex labex    0 Nov 13 17:34 file1.txt
-rw-rw-r-- 1 labex labex    0 Nov 13 17:34 file2.txt
drwxrwxr-x 3 labex labex   40 Nov 13 17:34 logs
-rwxr-xr-x 1 labex labex    0 Nov 13 17:34 script.py
labex:project/ $ ls -R
.:
data  document.md  file1.txt  file2.txt  logs  script.py

./data:

./logs:
archive  current.log

./logs/archive:
old.log
labex:project/ $  
```
![](Pasted%20image%2020261113114129.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this Lab i learned how powerful simple commands can be when you add flags/options to them. With the use of flags/options you can alter how the command executes allowing to get more accurate results.