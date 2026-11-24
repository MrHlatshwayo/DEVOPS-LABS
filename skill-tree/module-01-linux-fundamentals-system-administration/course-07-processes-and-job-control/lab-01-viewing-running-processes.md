# Lab: Viewing Running Processes

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, It will test us on our ability to view running processes.
- What problem were you tasked to solve?
  In this lab, I will check the "Order Rail" to see what is running.

---

## 🛠️ Commands & Configuration Used
```bash
ps (process status)
ps aux (process status- all,user, no terminal)
grep (search)
| (pipe)
```

---

## ✅ Results
- What was completed?
  I learned:
1. **Process**: A running program.
2. **PID**: The unique ticket number for every process.
3. **ps**: The command to see your own processes.
4. **ps aux**: The command to see _everything_.
5. **| grep**: How to filter the noise and find specifically what you are looking for.
- What output or verification confirmed success?
```
  labex         46  0.0  0.0  11212  3676 ?        S    20:20   0:00 sh -c { echo 'Running /home/labex/.vnc/xstartup'; /home/labex/.vnc/xstartup; } >> '/home/labex/.vnc/6b0
labex         47  0.0  0.0  11212  2224 ?        S    20:20   0:00 sh -c { echo 'Running /home/labex/.vnc/xstartup'; /home/labex/.vnc/xstartup; } >> '/home/labex/.vnc/6b0
labex         48  0.0  0.4 454072 77048 ?        Sl   20:20   0:00 xfce4-session
labex         57  0.0  0.0   8308  2596 ?        S    20:20   0:00 /usr/bin/dbus-launch --sh-syntax --exit-with-session xfce4-session
labex         58  0.0  0.0   8520  3456 ?        Ss   20:20   0:00 /usr/bin/dbus-daemon --syslog --fork --print-pid 5 --print-address 7 --session
labex         60  0.0  0.0 309468  8428 ?        Sl   20:20   0:00 /usr/libexec/at-spi-bus-launcher
labex         65  0.0  0.0   8432  4492 ?        S    20:20   0:00 /usr/bin/dbus-daemon --config-file=/usr/share/defaults/at-spi2/accessibility.conf --nofork --print-addr
labex         86  0.0  0.2 388996 39568 ?        Sl   20:20   0:00 xfwm4
labex         90  0.0  0.0 241752  8016 ?        Sl   20:20   0:00 /usr/libexec/gvfsd
labex        101  0.0  0.1 228016 25884 ?        Sl   20:20   0:00 xfsettingsd
labex        104  0.0  0.1 491388 30828 ?        Sl   20:20   0:00 xfce4-panel
labex        108  0.0  0.1 340552 22860 ?        Sl   20:20   0:00 Thunar --daemon
labex        113  0.0  0.3 473636 51768 ?        Sl   20:20   0:00 xfdesktop
labex        116  0.0  0.1 339776 23628 ?        Sl   20:20   0:00 /usr/lib/x86_64-linux-gnu/xfce4/panel/wrapper-2.0 /usr/lib/x86_64-linux-gnu/xfce4/panel/plugins/libsyst
labex        129  0.0  0.1 563584 23552 ?        SNl  20:20   0:00 /usr/lib/x86_64-linux-gnu/tumbler-1/tumblerd
labex        138  0.0  0.1 262944 18316 ?        Sl   20:20   0:00 /usr/lib/x86_64-linux-gnu/xfce4/notifyd/xfce4-notifyd
labex        140  0.0  0.1 189096 17808 ?        Sl   20:20   0:00 xfce4-power-manager
labex        143  0.0  0.0 159620  7392 ?        Sl   20:20   0:00 xiccd
labex        163  0.0  0.0 242288  8200 ?        Sl   20:20   0:00 /usr/libexec/gvfs-udisks2-volume-monitor
root         234  0.0  0.0  17156 11196 ?        Ss   20:20   0:00 sshd: labex [priv]
labex        245  0.0  0.0  17412  8200 ?        S    20:20   0:00 sshd: labex@notty
root         278  0.0  0.0   2644  1328 ?        S    20:20   0:00 dumb-init su - labex -c /usr/local/bin/ttyd -p 3002 -t fontSize=15 -t disableLeaveAlert=true -t titleFi
root         279  0.0  0.0  14072  5192 ?        Ss   20:20   0:00 su - labex -c /usr/local/bin/ttyd -p 3002 -t fontSize=15 -t disableLeaveAlert=true -t titleFixed=labex 
labex        280  0.0  0.0  10512  1880 ?        Rsl  20:20   0:00 /usr/local/bin/ttyd -p 3002 -t fontSize 15 -t disableLeaveAlert true -t titleFixed labex tmux new -As t
labex        287  0.0  0.0  12156  4284 pts/0    Ss+  20:20   0:00 tmux new -As ttyd -c /home/labex/project
labex        290  0.0  0.0  12548  4104 ?        Rs   20:20   0:00 tmux new -As ttyd -c /home/labex/project
labex        291  0.2  0.0   7636  6072 pts/1    Ss   20:20   0:00 -zsh
labex        293  0.2  0.0   7636  6108 pts/2    Ss   20:20   0:00 -zsh
labex        412  0.0  0.0   2808  1864 pts/1    S+   20:20   0:00 script -q -f /tmp/session/1795522852.log
labex        413  0.0  0.0   7392  5912 pts/3    Ss+  20:20   0:00 zsh -i
labex        421  0.0  0.0   2808  1864 pts/2    R+   20:20   0:00 script -q -f /tmp/session/1795522852.log
labex        422  0.0  0.0   7528  6040 pts/5    Ss   20:20   0:00 zsh -i
labex        596  0.0  0.0   7064  3104 pts/5    R+   20:23   0:00 ps aux
labex:project/ $ ps aux | grep sshd
root          22  0.0  0.0  15432  9664 ?        S    20:20   0:00 sshd: /usr/sbin/sshd -D [listener] 0 of 10-100 startups
root         234  0.0  0.0  17156 11196 ?        Ss   20:20   0:00 sshd: labex [priv]
labex        245  0.0  0.0  17412  8200 ?        S    20:20   0:00 sshd: labex@notty
labex        713  0.0  0.0   3472  2000 pts/5    S+   20:24   0:00 grep --color=auto --exclude-dir=.bzr --exclude-dir=CVS --exclude-dir=.git --exclude-dir=.hg --exclude-dir=.svn --exclude-dir=.idea --exclude-dir=.tox sshd
labex:project/ $ 
```
![](Pasted%20image%2020261124142725.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how to view processes in a Linux system and how to identify them using a PID.