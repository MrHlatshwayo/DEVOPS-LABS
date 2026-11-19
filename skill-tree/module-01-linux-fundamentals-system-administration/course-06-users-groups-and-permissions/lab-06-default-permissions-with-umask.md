# Lab: Default Permissions with umask

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will test our ability to configure permissions with umask
- What problem were you tasked to solve?
  I will adjust this "Cutter" to secure new files by default.
  Think of it like a **Cookie Cutter**.
1. **The Dough**: Maximum permissions (Read + Write).
2. **The Mask**: What you _remove_.
3. **The Cookie**: Final permissions.

---

## 🛠️ Commands & Configuration Used
```shell
umask (permisson filter)
ls (list)
```

---

## ✅ Results
- What was completed?
  I learned how Linux decides default permissions. I learned:
1. **Base Permissions**: Files start as `666` (Open to read/write).
2. **umask**: The "Mask" or "Filter" that removes permissions.
3. **002**: The default mask (Removes Write for others).
4. **077**: The private mask (Removes Everything for others).
- What output or verification confirmed success?
```
labex:project/ $ umask
002
labex:project/ $ touch default_file.txt
labex:project/ $ ls -l default_file.txt
-rw-rw-r-- 1 labex labex 0 Nov 19 15:02 default_file.txt
labex:project/ $ umask 077
labex:project/ $ umask
077
labex:project/ $ touch secure_file.txt
labex:project/ $ ls -l
total 0
-rw-rw-r-- 1 labex labex 0 Nov 19 15:02 default_file.txt
-rw------- 1 labex labex 0 Nov 19 15:03 secure_file.txt
labex:project/ $ 
```
![](Pasted%20image%2020261119090431.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how to configure files using umask and how that can help me to create templates for how every file permissions should be moving forward.