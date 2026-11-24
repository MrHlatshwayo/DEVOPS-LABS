# Lab: Process Priority with nice and renice

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will test our ability to change the priority of processes
- What problem were you tasked to solve?
  In this lab, I will manage "Niceness" to optimize performance.

---

## 🛠️ Commands & Configuration Used
```bash
nice (niceness)
renice (change niceness)
ps aux (process status, all, user,no terminal)
ps -l (process list)
pgrep (search process)
```

---

## ✅ Results
- What was completed?
  I learned:
1. **Niceness**: The "politeness" score of a process (-20 to 19).
2. **High Score = Low Priority**: Being nice means waiting your turn.
3. **nice**: Start a new program with a specific score.
4. **renice**: Change the score of a running program.
- What output or verification confirmed success?
```
labex:project/ $ sleep 3000 &
[1] 527
labex:project/ $ ps -l
F S   UID     PID    PPID  C PRI  NI ADDR SZ WCHAN  TTY          TIME CMD
4 S  5000     403     402  0  80   0 -  1882 sigsus pts/4    00:00:00 zsh
4 S  5000     527     403  0  85   5 -   698 hrtime pts/4    00:00:00 sleep
0 R  5000     536     403  0  80   0 -  1766 -      pts/4    00:00:00 ps
labex:project/ $ nice -n 10 sleep 4000 &
[2] 604
labex:project/ $ ps -l
F S   UID     PID    PPID  C PRI  NI ADDR SZ WCHAN  TTY          TIME CMD
4 S  5000     403     402  0  80   0 -  1882 sigsus pts/4    00:00:00 zsh
4 S  5000     527     403  0  85   5 -   698 hrtime pts/4    00:00:00 sleep
4 S  5000     604     403  0  95  15 -   698 hrtime pts/4    00:00:00 sleep
0 R  5000     613     403  0  80   0 -  1766 -      pts/4    00:00:00 ps
labex:project/ $ pgrep -f "sleep 3000"
527
labex:project/ $ renice -n 5 -p 527 
527 (process ID) old priority 5, new priority 5
labex:project/ $ ps -o pid,ni,comm
    PID  NI COMMAND
    403   0 zsh
    527   5 sleep
    604  15 sleep
    802   0 ps
labex:project/ $ 
```
![](Pasted%20image%2020261124152859.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
  In this lab I learned how to change the priority of processes, this is useful when dealing with multiple process that all require memory or CPU.