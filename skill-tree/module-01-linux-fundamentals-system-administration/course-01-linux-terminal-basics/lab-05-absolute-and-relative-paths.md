# Lab: Absolute and Relative Paths

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this Lab we will use the terminal, it tests us on command line shortcuts for Linux navigation
- What problem were you tasked to solve?
  1. **The Home Button**: `~`
  2. **The Root**: `/`
  3. **Relative Navigation**: "Go down here" vs "Go directly to X".
  4. **Climbing Up**: `..`
  5. **The Back Button**: `-`

---

## 🛠️ Commands & Configuration Used
```bash
pwd (print working directory)
ls (list all resources)
cd ~ (Teleport home)
cd / (go to root)
cd folder (go to folder)
cd .. (go to parent)
cd - (go to previous location)
```

---

## ✅ Results
- What was completed?
  I used command line shortcuts to navigate through the directory tree quicker such as:
  1. **`cd ~`**: Teleport Home.
  2. **`cd /`**: Go to the Root.
  3. **`cd folder`**: Step into a folder (Relative).
  4. **`cd ..`**: Step up to the parent (Up).
  5. **`cd -`**: Go back to the previous location (Back)..
- What output or verification confirmed success?
```
labex:project/ $ cd ~
labex:~/ $ pwd
/home/labex
labex:~/ $ cd /
labex:// $ ls
bin  boot  code-server_4.18.0_amd64.deb  data  dev  etc  home  lib  lib32  lib64  libx32  mariadb_repo_setup  media  mnt  opt  proc  root  run  sbin  snap  srv  sys  tmp  usr  var
labex:// $ cd home
labex:/home/ $ pwd
/home
labex:/home/ $ cd ..
labex:// $ pwd
/
labex:// $ cd -
/home
labex:/home/ $ cd -
/
labex:// $ 
```
![[Pasted image 20261112134622.png]]
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned the importance of knowing command line shortcuts and how they can make navigating to files quicker.
I also learned the difference between absolute paths `/` and relative paths.
Absolute paths start from the root directory and relative paths starts from the current directory you are working in.