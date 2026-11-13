# Lab: Linux Directory Structure Overview

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, testing us on our knowledge of the Linux operating system structure.
- What problem were you tasked to solve?
  We tasked with exploring the following:
  1. **The Root (`/`)**: This is the top of the tree. Everything starts here.
  2. **Branches (Directories)**: From the root, major branches grow out (like `bin`, `etc`, `home`).
  3. **Leaves (Files)**: At the end of the branches are the files.

---

## 🛠️ Commands & Configuration Used
```shell
/ (root directory)
/etc (editable text configuration directory)
/bin (binary directroy)
/home (home directory)
ls (list)
ls -F (list folder)
ls -@ (list link)
cat (print file)
which (where)

```

---

## ✅ Results
- What was completed?
  1. **The Tree Structure**: Linux files are organized in a single tree starting from Root (`/`).
  2. **The Root (`/`)**: The top of the hierarchy.
  3. **`/bin`**: The **Toolbox** where commands live.
  4. **`/etc`**: The **Settings** area for configurations.
  5. **`/home`**: Your **Personal Room** for files.
- What output or verification confirmed success?
The commands produced the expected outcomes
![](Pasted%20image%2020261113112224.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
This lab further expanded my knowledge of Linux system navigation. The main points are the following:
1. bin/ contains binary, and each command is just a program that is executed when prompted by the user
2. etc/ contains configuration files, these are the settings of the Linux operating systems
3. ls -F is used to list things in a folder
4. ls -@ is used to list things in a link
5. dev/ contains hardware devices such as storage
6. boot/ contains startup files
7. tmp/ contains temporary files 
8. user/ contains user programs and data