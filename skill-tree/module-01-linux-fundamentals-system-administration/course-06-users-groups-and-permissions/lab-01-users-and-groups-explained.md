# Lab: Users and Groups Explained

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it test our ability to view users and groups
- What problem were you tasked to solve?
1. **Users**: Tenants.
2. **Groups**: Access lists (Gym Group, Pool Group).

## 🛠️ Commands & Configuration Used
```bash
grep (search)
cat (show file)
id (identity of user)
```

---

## ✅ Results
- What was completed?
 I explored the "Who's Who" of your Linux system. You learned:
1. **Users** are defined in the `/etc/passwd` file.
2. **UID 0** belongs to `root`, the system administrator (Building Manager).
3. **UID 5000** is assigned to your user account in this system.
4. **Groups** control access to shared resources.
5. The `id` command shows your full identity, including which groups acting as "keys" you hold.
- What output or verification confirmed success?
```
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
labex:project/ $ grep "^root" /etc/passwd
root:x:0:0:root:/root:/bin/bash
labex:project/ $ grep "^labex" /etc/passwd
labex:x:5000:5000::/home/labex:/usr/bin/zsh
labex:project/ $ id
uid=5000(labex) gid=5000(labex) groups=5000(labex),27(sudo),121(ssl-cert),5002(public)
labex:project/ $ 
```
![](Pasted%20image%2020261118203128.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
Let's break down `labex:x:5000:5000::/home/labex:/usr/bin/zsh`:
1. **Username**: `labex`
2. **Password**: `x` (stored elsewhere)
3. **User ID (UID)**: `5000`
4. **Group ID (GID)**: `5000`
5. **Info**: (Empty)
6. **Home**: `/home/labex`
7. **Shell**: `/usr/bin/zsh`