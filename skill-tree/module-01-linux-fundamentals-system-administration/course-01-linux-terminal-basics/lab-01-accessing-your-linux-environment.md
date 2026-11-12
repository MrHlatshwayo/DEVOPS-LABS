# Lab: Accessing Your Linux Environment

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this Lab we taught how to interact with the terminal, this specific lab focused on our command line skills in Linux.
- What problem were you tasked to solve?
1. Distinguish between a standard user and the root user
2. Verify our current identity using the `whoami` command 
3. lastly to check the system's name using the `hostname` command.
---

## 🛠️ Commands & Configuration Used
```bash
whoami (reveals the identity of the user)
sudo -i (changes idenitity to root user)
exit (Exits from root user idenity)
pwd (prints the current directory Im working under)
hostname (shows the name of the system im logged on)
# Paste key commands or script snippets executed during the lab
```

---

## ✅ Results
- What was completed?
  1. **Terminal Access**: How to interact with the command line interface.
  2. **Prompts**: Understanding the difference between the standard user prompt (`$`) and the root user prompt (`#`).
  3. **Identity**: Using `whoami` to verify your username.
  4. **Location**: Using `pwd` to check your current directory.
  5. **System Info**: Using `hostname` to identify the machine.
- What output or verification confirmed success?
  Each command would print out the desired outcome, confirming prompts were correct
```Shell
labex:project/ $ whoami
labex
labex:project/ $ sudo -i
root@6af5619ad37ba9a2e8d7a597:~# exit
logout
labex:project/ $ pwd
/home/labex/project
labex:project/ $ hostname
6af5619ad37ba9a2e8d7a597
```
  ![[Pasted image 20261112085550.png]]

---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
What I learned is that the Command line is very character sensitive. For example I first typed `sudo i` instead of `sudo -i` and received an error before clearing the screen to start afresh.