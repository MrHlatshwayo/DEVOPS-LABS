# Lab: Foreground and Background Jobs

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will test our ability to keep track of jobs
- What problem were you tasked to solve?
  Control Jobs

---

## 🛠️ Commands & Configuration Used
```bash
jobs (view all jobs)
& (background job)
fg (foreground job)
```

---

## ✅ Results
- What was completed?
  I learned:
1. **Background (`&`)**: Start a command without blocking the terminal.
2. **Foreground (Default)**: Start a command that blocks the terminal.
3. **Suspend (`Ctrl+Z`)**: Pause the current foreground command.
4. **jobs**: List all your background/paused tasks.
5. **fg**: Bring a background task to the foreground.
- What output or verification confirmed success?
```
labex:project/ $ sleep 1000 &
[1] 638
labex:project/ $ sleep 2000
^Z
[2]  + 699 suspended  sleep 2000
labex:project/ $ jobs
[1]  - running    sleep 1000
[2]  + suspended  sleep 2000
labex:project/ $ fg %1
[1]  - 638 running    sleep 1000
^C
labex:project/ $ 
```
![](Pasted%20image%2020261124145628.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how to start and move processes in the foreground and backgroud.