# Lab: Removing Files and Directories Safely

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will test us on our ability to remove files and directories safely.
- What problem were you tasked to solve?
  1. Shred individual files (`rm`).
  2. Remove empty folders safely (`rmdir`).
  3. Force-delete full folders (`rm -rf`).

---

## 🛠️ Commands & Configuration Used
```bash
ls (list)
rm (remove)
ls -l (list long format)
rmdir (remove directory)
rmdir -rf (remove directory by force and recursively)
```

---

## ✅ Results
- What was completed?
  I have learned how to clean up my system.
1. `rm file`: The Shredder (for files).
2. `rmdir dir`: The Safe Removal (for empty folders).
3. `rm -rf dir`: The Bulldozer (for folders with content).
- What output or verification confirmed success?
```
labex:project/ $ ls
data_dir  empty_dir  file_to_delete.txt
labex:project/ $ rm file_to_delete.txt
labex:project/ $ ls -l
total 0
drwxrwxr-x 2 labex labex 40 Nov 14 01:18 data_dir
drwxrwxr-x 2 labex labex  6 Nov 14 01:18 empty_dir
labex:project/ $ rmdir empty_dir
labex:project/ $ ls -F
data_dir/
labex:project/ $ rmdir data_dir
rmdir: failed to remove 'data_dir': Directory not empty
labex:project/ $ rm -rf data_dir
labex:project/ $ ls
labex:project/ $ 
```
![](Pasted%20image%2020261113192137.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how to safely remove files and directories. Also how to remove a directory when it has files and folders inside of it.