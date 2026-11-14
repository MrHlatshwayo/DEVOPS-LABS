# Lab: Creating Custom Variables

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will test us on our ability to create custom variables. 
- What problem were you tasked to solve?
  1. Create a variable `MYCAFE`.
  2. Read its content.
  3. "Export" it.
  4. Verify it works in a second shell.

---

## 🛠️ Commands & Configuration Used
```bash
echo (print)
export (export variable)
bash (execute bash shell)
```

---

## ✅ Results
- What was completed?
  I practiced the lifecycle of a variable:
1. Creation: MYCAFE="espresso" (No spaces!)
2. Reading: echo $MYCAFE (Don't forget the $)
3. Sharing: export MYCAFE (Making it public to child processes)
- What output or verification confirmed success?
```SHELL
labex:project/ $ MYCAFE="espresso"
labex:project/ $ echo $MYCAFE 
espresso
labex:project/ $ export MYCAFE
labex:project/ $ bash
labex@6af859c268b2e3ec9acaf9c8:~/project$ echo $MYCAFE
espresso
labex@6af859c268b2e3ec9acaf9c8:~/project$ exit
exit
labex:project/ $  
```
![](Pasted%20image%2020261114150111.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how to create variables of my own and also how to execute in different shells by making them environment variables.