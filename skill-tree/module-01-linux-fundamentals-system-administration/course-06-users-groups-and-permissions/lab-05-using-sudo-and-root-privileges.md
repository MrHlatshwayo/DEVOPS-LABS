# Lab: Using sudo and Root Privileges

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will test our ability to use sudo and root privileges.
- What problem were you tasked to solve?
  

---

## 🛠️ Commands & Configuration Used
```bash
sudo (root privelege)
ls (list)
whoami (identity)
```

---

## ✅ Results
- What was completed?
  I learned to wield the power of the Superuser. I learned:
1. **Normal users** are blocked from sensitive files (like Password Vaults).
2. **sudo** allows you to temporarily execute commands as `root`.
3. **sudo -i** switches you into a full root session (Notice the `#` prompt!).
4. **exit** brings you back to safety.
- What output or verification confirmed success?
```
  sys:*:19901:0:99999:7:::
sync:*:19901:0:99999:7:::
games:*:19901:0:99999:7:::
man:*:19901:0:99999:7:::
lp:*:19901:0:99999:7:::
mail:*:19901:0:99999:7:::
news:*:19901:0:99999:7:::
uucp:*:19901:0:99999:7:::
proxy:*:19901:0:99999:7:::
www-data:*:19901:0:99999:7:::
backup:*:19901:0:99999:7:::
list:*:19901:0:99999:7:::
irc:*:19901:0:99999:7:::
gnats:*:19901:0:99999:7:::
nobody:*:19901:0:99999:7:::
_apt:*:19901:0:99999:7:::
systemd-network:*:19922:0:99999:7:::
systemd-resolve:*:19922:0:99999:7:::
messagebus:*:19922:0:99999:7:::
systemd-timesync:*:19922:0:99999:7:::
tcpdump:*:19922:0:99999:7:::
sshd:*:19922:0:99999:7:::
usbmux:*:19922:0:99999:7:::
rtkit:*:19922:0:99999:7:::
avahi:*:19922:0:99999:7:::
saned:*:19922:0:99999:7:::
colord:*:19922:0:99999:7:::
pulse:*:19922:0:99999:7:::
labex:$y$j9T$JO4YFYvYQW4BHNGvHSJ611$LRG/Fwi/EWDUCCOKqQ87Fi5pZmPZo/PRqshWGeI0FL2:20776:0:99999:7:::
mysql:!:19922:0:99999:7:::
mongodb:!:19922::::::
redis:*:19922:0:99999:7:::
labex:project/ $ sudo -i
root@6afe987368b2e3ec9ad6d2ef:~# whoami
root
root@6afe987368b2e3ec9ad6d2ef:~# exit
logout
labex:project/ $ whoami
labex
labex:project/ $ 
```
![](Pasted%20image%2020261119085644.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab i learned how powerful sudo can be and how to access root priveleges when needed.