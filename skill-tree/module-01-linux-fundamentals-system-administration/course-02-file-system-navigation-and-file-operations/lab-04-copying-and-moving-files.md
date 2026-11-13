# Lab: Copying and Moving Files

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will using the terminal, we will be tested on our ability to copy an move files in the CLI
- What problem were you tasked to solve?
  1. duplicate files,
  2. clone entire directories,
  3. and organize your workspace
---

## 🛠️ Commands & Configuration Used
```shell
cp (copy)
cp -r (copy recursively)
mv (move/rename)
ls (list)
ls -F (list folder)
```

---

## ✅ Results
- What was completed?
  1. **`cp file new_file`**: Copy a file.
  2. **`cp -r dir new_dir`**: Copy a directory (Recursive).
  3. **`mv old new`**: Rename a file.
  4. **`mv file dir/`**: Move a file into a folder.
- What output or verification confirmed success?
```
labex:project/ $ ls 
file1.txt  project_alpha
labex:project/ $ cp file1.txt file1.bak
labex:project/ $ ls
file1.bak  file1.txt  project_alpha
labex:project/ $ cp -r project_alpha project_beta
labex:project/ $ ls -F
file1.bak  file1.txt  project_alpha/  project_beta/
labex:project/ $ mv file1.bak file1.old
labex:project/ $ ls
file1.old  file1.txt  project_alpha  project_beta
labex:project/ $ mv file1.old project_alpha/
labex:project/ $ ls
file1.txt  project_alpha  project_beta
labex:project/ $ ls project_alpha/
data.txt  file1.old
labex:project/ $ 
```
![](Pasted%20image%2020261113120351.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
What I learned in this lab is how to move, copy and rename files and directories. What stood for is the logic behind both moving and renaming having the same command, at the core they bot edit the details of the file wether path or just title.

What I still wanna test is if moving a directory into another directory is simple or would also need me to use the recursive flag.