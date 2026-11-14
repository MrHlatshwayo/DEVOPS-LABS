# Lab: Pipes and Chaining Commands

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will be testing us on our ability use pipes and chaining commands
- What problem were you tasked to solve?
  In this lab, I will build your own data processing assembly lines using pipes.

---

## 🛠️ Commands & Configuration Used
```bash
| (pipe/connects commands)
ls (list)
wc -l (count lines)
```

---

## ✅ Results
- What was completed?
  In this lab, I learned to play the role of a data plumber using **Pipes (`|`)**:
1. **Connecting Tools**: You learned that output from one command can become input for another.
2. **Building Pipelines**: You chained commands like `ls`, `cat`, `grep`, and `wc` to create custom data processing streams.
- What output or verification confirmed success?
``` 
labex:project/ $ cd data
labex:data/ $ ls | wc -l        
7
labex:data/ $ cat linux_info.txt | grep "Linux"
Linux is an open source operating system.
Learning Linux is a great skill.
labex:data/ $ cat linux_info.txt | grep "is" | wc -l
5
labex:data/ $ 
```
![](Pasted%20image%2020261114095809.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned to connect commands, basically directing the output of one command to be the input of another command and thereby altering the overall output command of the prompt.