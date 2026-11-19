# Lab: Changing Permissions with Symbolic and Octal Modes

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will test our ability to change permissions with symbolic and octaval modes.
- What problem were you tasked to solve?
  In this lab, I will use both to secure a script.

---

## 🛠️ Commands & Configuration Used
```bash
echo (print output)
ls -l (list long format)
chmod (change permissions)
```

---

## ✅ Results
- What was completed?
  I learned how to control access. I learned:
1. **Symbolic Mode** (`chmod +x`): Best for adding/removing specific rights without changing others.
2. **Octal Mode** (`chmod 600`): Best for setting a definitive security policy from scratch.
3. **Security**: The importance of removing permissions for "Others" to protect secrets.
- What output or verification confirmed success?
```
labex:project/ $ echo 'echo "Hello, LabEx!"' > runme.sh
labex:project/ $ ls -l runme.sh
-rw-rw-r-- 1 labex labex 21 Nov 19 14:16 runme.sh
labex:project/ $ chmod +x runme.sh
labex:project/ $ ls -l runme.sh
-rwxrwxr-x 1 labex labex 21 Nov 19 14:16 runme.sh
labex:project/ $ chmod o-r runme.sh
labex:project/ $ ls -l
total 4
-rwxrwx--x 1 labex labex 21 Nov 19 14:16 runme.sh
labex:project/ $ chmod 600 runme.sh
labex:project/ $ ls -l
total 4
-rw------- 1 labex labex 21 Nov 19 14:16 runme.sh
labex:project/ $ 
 
```
![](Pasted%20image%2020261119083251.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this file I learned how to edit permissions in a systematic way.