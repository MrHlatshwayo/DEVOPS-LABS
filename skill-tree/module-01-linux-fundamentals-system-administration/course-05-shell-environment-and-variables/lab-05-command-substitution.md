# Lab: Command Substitution

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, This lab will test our ability to use command substitution in the CLI
- What problem were you tasked to solve?
  1. Learn how to format the `date` command.
  2. Create a folder that is automatically named with today's date (e.g., `2025-12-23`)

---

## 🛠️ Commands & Configuration Used
```SHELL
date (date)
mkdir (make directory)
$() (command substituiton)
```

---

## ✅ Results
- What was completed?
   I learned about **Command Substitution**—the art of using the output of one command as the input for another.
1. **The Trick**: `$(command)`
2. **The Process**: Linux runs the inner command first, then swaps it with the result.
3. **The Result**: You can create dynamic commands that change based on time, user, or other conditions without typing them manually.
- What output or verification confirmed success?
```
labex:project/ $ date +%F
2026-11-14
labex:project/ $ mkdir $(date +%F)
labex:project/ $ ls -l
total 0
drwxrwxr-x 2 labex labex 6 Nov 14 21:29 2026-11-14
labex:project/ $ 
```
![](Pasted%20image%2020261114153017.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how to substitute commands which is very usefull and more efficient than building pipelines.