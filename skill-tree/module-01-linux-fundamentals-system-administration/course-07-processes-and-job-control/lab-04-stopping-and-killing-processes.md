# Lab: Stopping and Killing Processes

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it test our ability to stop and kill processes
- What problem were you tasked to solve?
  In this lab, I will stop unresponsive programs safely.

---

## 🛠️ Commands & Configuration Used
```bash
kill (polite kill)
kill -9 (force kill)
pkill -f (kill by name)
```

---

## ✅ Results
- What was completed?
  I learned:
1. **kill** : The polite way to stop a specific process (SIGTERM).
2. **kill -9** : The forceful way to destroy a frozen process (SIGKILL).
3. **pkill** : The shortcut to kill by name without looking up the number.
- What output or verification confirmed success?
```
labex:project/ $ ./bad_process.sh &
[1] 815
labex:project/ $ ps aux | grep bad_process.sh
labex        815  0.0  0.0   4496  3464 pts/4    SN   21:16   0:00 /bin/bash ./bad_process.sh
labex        919  0.0  0.0   3472  1876 pts/4    R+   21:16   0:00 grep --color=auto --exclude-dir=.bzr --exclude-dir=CVS --exclude-dir=.git --exclude-dir=.hg --exclude-dir=.svn --exclude-dir=.idea --exclude-dir=.tox bad_process.sh
labex:project/ $ kill 815
[1]  + 815 terminated  ./bad_process.sh                                                                                                                                   
labex:project/ $ jobs
labex:project/ $ ./stubborn_process.sh &
[1] 1088
labex:project/ $ kill 1088
labex:project/ $ I refuse to stop!
kill -p 1088
kill: unknown signal: SIGP
kill: type kill -l for a list of signals
labex:project/ $ kill -9 1088
[1]  + 1088 killed     ./stubborn_process.sh                                                                                                                              
labex:project/ $ jobs
labex:project/ $ ./bad_process.sh &
[1] 1286
labex:project/ $ pkill -f bad_process.sh
[1]  + 1286 terminated  ./bad_process.sh
labex:project/ $ jobs
labex:project/ $ 
```
![](Pasted%20image%2020261124152002.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
  In this lab I learned how to stop and kill processes, both those stop willingly and those unwilling to stop.