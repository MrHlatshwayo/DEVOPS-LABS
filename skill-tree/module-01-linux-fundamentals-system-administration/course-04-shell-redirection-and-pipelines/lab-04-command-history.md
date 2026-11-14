# Lab: Command History

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will test our ability to view the command history
- What problem were you tasked to solve?
  In this lab, I will learn how to access this logbook, replay my recent actions, and search through my past.

---

## 🛠️ Commands & Configuration Used
```bash
history (show command history)
ls (list)
whoami (user identity)
grep (search)
!! (previous command)
```

---

## ✅ Results
- What was completed?
  In this lab, I learned that I never have to rely solely on my memory. Linux remembers for me.
- **`history`**: Your logbook of past actions.
- **`!!`**: The "Repeat" button for the last command.
- **`Ctrl+R`**: The "Search" function to find old commands instantly.
- What output or verification confirmed success?
```
  labex:project/ $ grep "bin" /etc/passwd
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
uucp:x:10:10:uucp:/var/spool/uucp:/usr/sbin/nologin
proxy:x:13:13:proxy:/bin:/usr/sbin/nologin
www-data:x:33:33:www-data:/var/www:/usr/sbin/nologin
backup:x:34:34:backup:/var/backups:/usr/sbin/nologin
list:x:38:38:Mailing List Manager:/var/list:/usr/sbin/nologin
irc:x:39:39:ircd:/run/ircd:/usr/sbin/nologin
gnats:x:41:41:Gnats Bug-Reporting System (admin):/var/lib/gnats:/usr/sbin/nologin
nobody:x:65534:65534:nobody:/nonexistent:/usr/sbin/nologin
_apt:x:100:65534::/nonexistent:/usr/sbin/nologin
systemd-network:x:101:102:systemd Network Management,,,:/run/systemd:/usr/sbin/nologin
systemd-resolve:x:102:103:systemd Resolver,,,:/run/systemd:/usr/sbin/nologin
messagebus:x:103:109::/nonexistent:/usr/sbin/nologin
systemd-timesync:x:104:110:systemd Time Synchronization,,,:/run/systemd:/usr/sbin/nologin
tcpdump:x:105:111::/nonexistent:/usr/sbin/nologin
sshd:x:106:65534::/run/sshd:/usr/sbin/nologin
usbmux:x:107:46:usbmux daemon,,,:/var/lib/usbmux:/usr/sbin/nologin
rtkit:x:108:113:RealtimeKit,,,:/proc:/usr/sbin/nologin
avahi:x:109:114:Avahi mDNS daemon,,,:/run/avahi-daemon:/usr/sbin/nologin
saned:x:110:117::/var/lib/saned:/usr/sbin/nologin
colord:x:111:118:colord colour management daemon,,,:/var/lib/colord:/usr/sbin/nologin
pulse:x:112:119:PulseAudio daemon,,,:/run/pulse:/usr/sbin/nologin
labex:x:5000:5000::/home/labex:/usr/bin/zsh
mysql:x:113:122:MySQL Server,,,:/var/lib/mysql/:/bin/false
mongodb:x:999:999::/home/mongodb:/bin/sh
redis:x:114:123::/var/lib/redis:/usr/sbin/nologin
labex:project/ $ grep "root" /etc/passwd
root:x:0:0:root:/root:/bin/bash
labex:project/ $ 
```
![](Pasted%20image%2020261114100652.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab i learned command that would me recall command used without actually having to remember myself. This is great for auditing my steps and fore efficiently using a previous command without retyping.