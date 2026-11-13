# Lab: Viewing Files with Head Tail and Cat

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will be testing our ability to view files with head, tail and cate.
- What problem were you tasked to solve?
  1. **`cat`**: Reads the entire file at once. Best for small notes.
  2. **`head`**: Reads just the beginning (the "headline"). Best for checking what a file is about.
  3. **`tail`**: Reads just the end. Best for checking the latest updates in a log file.

---

## 🛠️ Commands & Configuration Used
```bash
cat (concatenate)
head (first 10 lines)
tail (last 10 lines)
tail -f (tail follow)
ls (list)
```

---

## ✅ Results
- What was completed?
  - **`cat`**: Reads the whole file. Good for small files.
- **`head`**: Reads the beginning. Good for quick checks.
- **`tail`**: Reads the end. Good for logs.
- **`tail -f`**: Watches a file in real-time.
- What output or verification confirmed success?
```
Line 5: End of the sample file.
labex:project/ $ head /etc/passwd
root:x:0:0:root:/root:/bin/bash
daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
bin:x:2:2:bin:/bin:/usr/sbin/nologin
sys:x:3:3:sys:/dev:/usr/sbin/nologin
sync:x:4:65534:sync:/bin:/bin/sync
games:x:5:60:games:/usr/games:/usr/sbin/nologin
man:x:6:12:man:/var/cache/man:/usr/sbin/nologin
lp:x:7:7:lp:/var/spool/lpd:/usr/sbin/nologin
mail:x:8:8:mail:/var/mail:/usr/sbin/nologin
news:x:9:9:news:/var/spool/news:/usr/sbin/nologin
labex:project/ $ head -n 5 /etc/passwd
root:x:0:0:root:/root:/bin/bash
daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
bin:x:2:2:bin:/bin:/usr/sbin/nologin
sys:x:3:3:sys:/dev:/usr/sbin/nologin
sync:x:4:65534:sync:/bin:/bin/sync
labex:project/ $ tail /var/log/syslog
Sat Nov 14 01:45:16 CST 2026 LabEx-VM systemd[1]: Sample log entry 41 generated for testing tail command
Sat Nov 14 01:45:16 CST 2026 LabEx-VM systemd[1]: Sample log entry 42 generated for testing tail command
Sat Nov 14 01:45:16 CST 2026 LabEx-VM systemd[1]: Sample log entry 43 generated for testing tail command
Sat Nov 14 01:45:16 CST 2026 LabEx-VM systemd[1]: Sample log entry 44 generated for testing tail command
Sat Nov 14 01:45:16 CST 2026 LabEx-VM systemd[1]: Sample log entry 45 generated for testing tail command
Sat Nov 14 01:45:16 CST 2026 LabEx-VM systemd[1]: Sample log entry 46 generated for testing tail command
Sat Nov 14 01:45:16 CST 2026 LabEx-VM systemd[1]: Sample log entry 47 generated for testing tail command
Sat Nov 14 01:45:16 CST 2026 LabEx-VM systemd[1]: Sample log entry 48 generated for testing tail command
Sat Nov 14 01:45:16 CST 2026 LabEx-VM systemd[1]: Sample log entry 49 generated for testing tail command
Sat Nov 14 01:45:16 CST 2026 LabEx-VM systemd[1]: Sample log entry 50 generated for testing tail command
labex:project/ $ tail -n 5 /var/log/syslog
Sat Nov 14 01:45:16 CST 2026 LabEx-VM systemd[1]: Sample log entry 46 generated for testing tail command
Sat Nov 14 01:45:16 CST 2026 LabEx-VM systemd[1]: Sample log entry 47 generated for testing tail command
Sat Nov 14 01:45:16 CST 2026 LabEx-VM systemd[1]: Sample log entry 48 generated for testing tail command
Sat Nov 14 01:45:16 CST 2026 LabEx-VM systemd[1]: Sample log entry 49 generated for testing tail command
Sat Nov 14 01:45:16 CST 2026 LabEx-VM systemd[1]: Sample log entry 50 generated for testing tail command
labex:project/ $ tail -f ~/project/app.log
labex:project/ $ tail -f ~/project/app.log
New log entry at Sat Nov 14 01:54:44 CST 2026
Another event happened
System is running smoothly

```
![](Pasted%20image%2020261113195602.png)


## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how to use head and tail which is very useful when I have to view specific content in a file. More especially using the tail -f command to get live updates on a log file.