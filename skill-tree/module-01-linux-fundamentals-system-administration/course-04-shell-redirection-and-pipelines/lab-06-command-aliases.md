# Lab: Command Aliases

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will test our ability to use command aliases
- What problem were you tasked to solve?
  In this lab, I will learn how to create my own custom command shortcuts.
---

## 🛠️ Commands & Configuration Used
```shell
alias (command shortcut)
unalias (delete command shortcut)
ls (list)
```

---

## ✅ Results
- What was completed?
  In this lab, I learned how to create my own command shortcuts using **Aliases**:
1. **`alias name='command'`**: create a new nickname.
2. **`unalias name`**: delete a nickname.
- What output or verification confirmed success?
```
labex:project/ $ ll 
total 4.0K
drwxr-xr-x 1 labex labex   68 Nov 14 16:17 .
drwxr-x--- 1 labex labex 4.0K Nov 14 16:21 ..
-rw-rw-r-- 1 labex labex    0 Nov 14 16:17 .hidden_config
-rw-rw-r-- 1 labex labex    0 Nov 14 16:17 data.log
-rw-rw-r-- 1 labex labex    0 Nov 14 16:17 example_file.txt
labex:project/ $ unalias ll
labex:project/ $ ll
zsh: command not found: ll
labex:project/ $ 
```
![](Pasted%20image%2020261114102244.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how to create command shortcuts, this makes it easier to use certain command during my session to save myself time to type out the whole thing.