# Lab: Environment Setup Script

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, we will be tested on our ability to setup environment using CLI.
- What problem were you tasked to solve?
  1. **Define** a persistent variable for your project path.
2. **Create** an alias to jump there instantly.
3. **Persist** these changes so they work every time.

---

## 🛠️ Commands & Configuration Used
```bash
vim (text editor)
source (reload shell)
cd (change directroy)
```

---

## ✅ Results
- What was completed?
  In this challenge, I:
1. **Defined Variables**: Created `PROJECT_DIR`.
2. **Created Aliases**: Built `goto_proj`.
3. **Managed State**: Used `source` to apply changes.
- What output or verification confirmed success?
```
labex:project/ $ vim ~/.zshrc
labex:project/ $ vim ~/.zshrc
labex:project/ $ source ~/.zshrc
labex:project/ $ cd /tmp
labex:/tmp/ $ goto_proj
labex:project/ $ pwd
/home/labex/project
labex:project/ $ 
```
![](Pasted%20image%2020261114154511.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how to configure my shell environment and how to setup persistent alias commands