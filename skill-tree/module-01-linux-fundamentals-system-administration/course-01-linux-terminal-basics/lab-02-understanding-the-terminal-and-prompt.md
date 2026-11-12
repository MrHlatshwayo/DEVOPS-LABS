# Lab: Understanding the Terminal and Prompt

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we'll be using the terminal, further testing our command line skills in Linux
- What problem were you tasked to solve?
1. **Decode the Prompt**: Understand the meaning of `labex:project/ $`.
2. **Speak to the System**: Use the `echo` command to print text and variable values.
3. **Keep it Tidy**: Use the `clear` command to organize your workspace to avoid clutter.
---

## 🛠️ Commands & Configuration Used
```shell
whoami (reveals identity of user)
pwd (prints current working directory)
echo (prints an ouput to a screen)
clear (clears all information on the screen)
Ctrl + L (shortcut for clear)
```

---

## ✅ Results
- What was completed?
1. **Reading the Prompt**: You can now decode `labex:project/ $` to understand your user, location, and privileges.
2. **Echoing Text**: You learned to use `echo` to print messages and display variable values like `$USER`.
3. **Clearing the Screen**: You know how to keep your workspace tidy using `clear` or the **Ctrl + L** shortcut.
- What output or verification confirmed success?
  Each prompt would print the desired outcome
```
labex:project/ $ whoami
labex
labex:project/ $ pwd
/home/labex/project
labex:project/ $ echo "Hello World"
Hello World
labex:project/ $ echo "I am logged in as $USER"
I am logged in as labex
labex:project/ $ 
```
![Terminal prompt example](../../Pasted%20image%2020261112092317.png)
---
![Terminal prompt details](../../Pasted%20image%2020261112092737.png)
## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
 What I learned today was how prompts are structured and how being able the read them helps me have a better understanding of the user, location and privileges.
 `labex:project/ $`
 `labex` = User/Username
 `project/` = working directory/location
 `$` = standard user
 `#` = root user