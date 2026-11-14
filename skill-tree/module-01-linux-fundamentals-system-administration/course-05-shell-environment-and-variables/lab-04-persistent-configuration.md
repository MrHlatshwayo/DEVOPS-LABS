# Lab: Persistent Configuration

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, It will test our ability to make persistent configs in the CLI
- What problem were you tasked to solve?
  1. Modify **Zsh** config.
  2. Switch to **Bash**.
  3. Modify **Bash** config.

---

## 🛠️ Commands & Configuration Used
```bash
nano (text editor)
source (reload shell)
bash (open bash shell)
```

---

## ✅ Results
- What was completed?
  I learned how to personalize my Linux environment permanently:
1. **Shell Specifics**: Different shells (Zsh, Bash) use different configuration files (`.zshrc`, `.bashrc`).
2. **Persistence**: Changes made in a terminal session are temporary unless saved to these files.
3. **Source**: Using `source` allows you to apply changes immediately without restarting the terminal.
- What output or verification confirmed success?
```
labex:project/ $ nano ~/.zshrc
labex:project/ $ source ~/.zshrc
labex:project/ $ hellozsh
Hello from Zsh
labex:project/ $ bash 
labex@6af85bf968b2e3ec9acafdbb:~/project$ hellozsh
bash: hellozsh: command not found
labex@6af85bf968b2e3ec9acafdbb:~/project$ nano ~/.bashrc
labex@6af85bf968b2e3ec9acafdbb:~/project$ source ~/.bashrc
labex@6af85bf968b2e3ec9acafdbb:~/project$ hellobash
Hello from Bash
labex@6af85bf968b2e3ec9acafdbb:~/project$ exit
exit
labex:project/ $ 
```
![](Pasted%20image%2020261114152307.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how to configure my shell environment in way that is persistent and not session bound, this useful when i need to make permanent changes.