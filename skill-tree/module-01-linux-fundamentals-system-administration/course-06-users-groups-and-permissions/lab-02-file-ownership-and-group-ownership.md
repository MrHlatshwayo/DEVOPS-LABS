# Lab: File Ownership and Group Ownership

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will test our ability to view and transfer ownership of files.
- What problem were you tasked to solve?
  I will check ownership and transfer it to others.

---

## 🛠️ Commands & Configuration Used
```bash
cd (change directory)
chown (change owner)
sudo (admin privelege)
chgrp (change group)
ls (list)
ls -l (list long format)
```

---

## ✅ Results
- What was completed?
  I learned:
1. **Everything has an owner**: Every file has a User Owner and a Group Owner.
2. **ls -l**: The command to see these ownership labels.
3. **chown**: The command to change the **User** owner.
4. **chgrp**: The command to change the **Group** owner.
- What output or verification confirmed success?
```
labex:project/ $ cd ~/project
labex:project/ $ touch test_owner.txt
labex:project/ $ ls
test_owner.txt
labex:project/ $ ls -l
total 0
-rw-rw-r-- 1 labex labex 0 Nov 19 13:54 test_owner.txt
labex:project/ $ sudo chown root test_owner.txt
labex:project/ $ ls -l
total 0
-rw-rw-r-- 1 root labex 0 Nov 19 13:54 test_owner.txt
labex:project/ $ sudo chgrp root test_owner.txt
labex:project/ $ ls -l
total 0
-rw-rw-r-- 1 root root 0 Nov 19 13:54 test_owner.txt
labex:project/ $ 
```
![](Pasted%20image%2020261119075717.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how every file has an owner, also how to transfer the ownership of a file to another user should it be necessary. 