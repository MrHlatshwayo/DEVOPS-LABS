# Lab: Real-time Monitoring with top

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will use the terminal, it will test our ability to do view processes in real time
- What problem were you tasked to solve?
  In this lab, I will catch resource-hungry apps in the act.

---

## 🛠️ Commands & Configuration Used
```bash
top (live process view)
echo (print file)
cat (show file)
```

---

## ✅ Results
- What was completed?
  I learned:
1. **top**: The command to see real-time system stats.
2. **Shift + M**: Sort by Memory (Find the RAM hogs).
3. **Shift + P**: Sort by CPU (Find the Processor hogs).
4. **q**: Quit the dashboard.
- What output or verification confirmed success?
```
  
top - 20:33:38 up 2 days,  1:28,  0 users,  load average: 0.25, 0.31, 0.29
Tasks:  44 total,   1 running,  43 sleeping,   0 stopped,   0 zombie
top - 20:36:27 up 2 days,  1:31,  0 users,  load average: 1.22, 0.52, 0.36
Tasks:  43 total,   1 running,  42 sleeping,   0 stopped,   0 zombie
%Cpu(s):  8.2 us,  0.6 sy,  0.0 ni, 91.1 id,  0.0 wa,  0.0 hi,  0.1 si,  0.0 st
MiB Mem :  15322.5 total,   4392.3 free,   5012.6 used,   5917.6 buff/cache
MiB Swap:      0.0 total,      0.0 free,      0.0 used.   9892.2 avail Mem 

    PID USER      PR  NI    VIRT    RES    SHR S  %CPU  %MEM     TIME+ COMMAND                                                                                            
    209 labex     20   0   72784  60768   5820 S  18.0   0.4   0:59.12 python3                                                                                            
      1 root      20   0   11212   3820   3536 S   0.0   0.0   0:00.00 init.sh                                                                                            
     21 root      20   0   40832  28344  10812 S   0.0   0.2   0:00.17 supervisord                                                                                        
     22 root      20   0   15432   9460   7824 S   0.0   0.1   0:00.00 sshd                                                                                               
     23 root      20   0   14048   5048   4476 S   0.0   0.0   0:00.00 su                                                                                                 
     24 labex     20   0   40324  30656   6588 S   0.0   0.2   0:00.38 vncserver                                                                                          
     36 labex     20   0  313944  83208  54336 S   0.0   0.5   0:00.26 Xvnc                                                                                               
     46 labex     20   0   11212   3552   3300 S   0.0   0.0   0:00.00 sh                                                                                                 
     47 labex     20   0   11212   2276   1996 S   0.0   0.0   0:00.00 sh                                                                                                 
     48 labex     20   0  454084  77548  61748 S   0.0   0.5   0:00.13 xfce4-session                                                                                      
     57 labex     20   0    8308   2540   2076 S   0.0   0.0   0:00.00 dbus-launch                                                                                        
     58 labex     20   0    8524   3376   2728 S   0.0   0.0   0:00.02 dbus-daemon                                                                                        
     60 labex     20   0  309468   8384   7464 S   0.0   0.1   0:00.00 at-spi-bus-laun                                                                                    
     65 labex     20   0    8432   4532   4040 S   0.0   0.0   0:00.00 dbus-daemon                                                                                        
     69 labex     20   0  231008   6712   5836 S   0.0   0.0   0:00.02 xfconfd                                                                                            
     75 labex     20   0  162756   8436   7568 S   0.0   0.1   0:00.00 at-spi2-registr                                                                                    
     80 labex     20   0    7980   2108   1028 S   0.0   0.0   0:00.00 ssh-agent                                                                                          
     85 labex     20   0   11504   2244   1956 S   0.0   0.0   0:00.00 gpg-agent                                                                                          
     86 labex     20   0  388936  39348  32192 S   0.0   0.3   0:00.10 xfwm4                                                                                              
     90 labex     20   0  241752   8192   7332 S   0.0   0.1   0:00.00 gvfsd                                                                                              
    101 labex     20   0  227988  25776  19860 S   0.0   0.2   0:00.07 xfsettingsd                                                                                        
    104 labex     20   0  417652  30656  24764 S   0.0   0.2   0:00.07 xfce4-panel                                                                                        
    108 labex     20   0  340488  23156  18256 S   0.0   0.1   0:00.03 Thunar                                                                                             
    113 labex     20   0  473640  51908  34528 S   0.0   0.3   0:00.19 xfdesktop                                                                                          
    116 labex     20   0  339768  23560  18696 S   0.0   0.2   0:00.03 panel-6-systray                                                                                    
    136 labex     20   0  262952  18892  16616 S   0.0   0.1   0:00.01 xfce4-notifyd                                                                                      
labex:project/ $ echo "209" > ~/project/hog_pid.txt
labex:project/ $ cat ~/project/hog_pid.txt 
209
labex:project/ $ 
```
![](Pasted%20image%2020261124143800.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how to view files in real time, this is useful to find memory intensive programs and cpu intensive programs.