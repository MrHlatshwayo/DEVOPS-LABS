# Lab: Creating Files and Directories

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this Lab we will be using the terminal, it will be testing us on our ability to create files and directories using the CLI. 
- What problem were you tasked to solve?
  1. Create new empty files.
  2. Build folders (directories) to organize your work.
  3. Construct entire directory paths in a single command.

---

## 🛠️ Commands & Configuration Used
```shell
touch (create/update file)
ls (list)
ls -F (list folder)
ls -R (list recursively)
mkdir (make directory)
mkdir -p (make parent directroy and child)
```

---

## ✅ Results
- What was completed?
  1. **`touch filename`**: Creates an empty file (or updates the timestamp of an existing one).
  2. **`mkdir directoryname`**: Creates a new directory.
  3. **`mkdir -p path/to/directory`**: Creates a full path of directories, building any missing parents automatically.
- What output or verification confirmed success?
```
labex:project/ $ touch file1.txt
labex:project/ $ ls -l
total 0
-rw-rw-r-- 1 labex labex 0 Nov 13 17:49 file1.txt
labex:project/ $ mkdir project_alpha
labex:project/ $ ls -F
file1.txt  project_alpha/
labex:project/ $ mkdir -p logs/labexio/jan
labex:project/ $ ls -R logs
logs:
labexio

logs/labexio:
jan

logs/labexio/jan:
labex:project/ $ 
```
  ![](Pasted%20image%2020261113115258.png)

---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how to create files and directories. What stood out the most is how i can make a nested directory using the `mkdir -p` command.