# Lab: Runaway Process Mitigation

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will test our ability to use all the skills covered in this course.
- What problem were you tasked to solve?
1. Connect to the server.
2. Identify the rogue process.
3. Terminate it to restore stability.
---

## 🛠️ Commands & Configuration Used
```bash
& (background process)
top (view processes in real time)
pgrep (search processes)
kill -9 (kill processes by force)
```

---

## ✅ Results
- What was completed?
  I practiced:
1. **Starting Jobs**: `&`.
2. **Monitoring**: `top`.
3. **Finding PIDs**: `pgrep`.
4. **Lifecycle**: Polite `kill` vs Force `kill -9`.
- What output or verification confirmed success?
```
top - 21:35:31 up 2 days,  2:30,  0 users,  load average: 0.66, 0.52, 0.59
Tasks:  43 total,   2 running,  41 sleeping,   0 stopped,   0 zombie
%Cpu(s):  1.2 us,  0.1 sy, 25.0 ni, 73.7 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st
MiB Mem :  15322.5 total,   3306.0 free,   4499.8 used,   7516.7 buff/cache
MiB Swap:      0.0 total,      0.0 free,      0.0 used.  10404.5 avail Mem 

    PID USER      PR  NI    VIRT    RES    SHR S  %CPU  %MEM     TIME+ COMMAND                                                                                            
    609 labex     25   5    4364   3100   2844 R 100.0   0.0   0:45.00 bad_process.sh                                                                                     
      1 root      20   0   11212   3772   3484 S   0.0   0.0   0:00.00 init.sh                                                                                            
     21 root      20   0   40832  28456  10928 S   0.0   0.2   0:00.16 supervisord                                                                                        
     22 root      20   0   15432   9584   7952 S   0.0   0.1   0:00.00 sshd                                                                                               
     23 root      20   0   14048   4972   4396 S   0.0   0.0   0:00.00 su                                                                                                 
     24 labex     20   0   40336  30732   6652 S   0.0   0.2   0:00.40 vncserver                                                                                          
     36 labex     20   0  310876  79988  54164 S   0.0   0.5   0:00.28 Xvnc                                                                                               
     46 labex     20   0   11212   3540   3292 S   0.0   0.0   0:00.00 sh                                                                                                 
     47 labex     20   0   11212   2276   2000 S   0.0   0.0   0:00.00 sh                                                                                                 
     48 labex     20   0  454072  76828  61024 S   0.0   0.5   0:00.14 xfce4-session                                                                                      
     57 labex     20   0    8308   2680   2220 S   0.0   0.0   0:00.00 dbus-launch                                                                                        
     58 labex     20   0    8524   3480   2820 S   0.0   0.0   0:00.02 dbus-daemon                                                                                        
     60 labex     20   0  309600   8580   7664 S   0.0   0.1   0:00.00 at-spi-bus-laun                                                                                    
     65 labex     20   0    8432   4604   4112 S   0.0   0.0   0:00.00 dbus-daemon                                                                                        
     69 labex     20   0  231008   6500   5628 S   0.0   0.0   0:00.03 xfconfd                                                                                            
     74 labex     20   0  162756   8436   7564 S   0.0   0.1   0:00.00 at-spi2-registr                                                                                    
     80 labex     20   0    7980   2284   1204 S   0.0   0.0   0:00.00 ssh-agent                                                                                          
     85 labex     20   0   11504   2192   1904 S   0.0   0.0   0:00.00 gpg-agent                                                                                          
     86 labex     20   0  388948  39408  32244 S   0.0   0.3   0:00.11 xfwm4                                                                                              
     90 labex     20   0  241884   8312   7456 S   0.0   0.1   0:00.00 gvfsd                                                                                              
    101 labex     20   0  228000  25972  20068 S   0.0   0.2   0:00.07 xfsettingsd                                                                                        
    104 labex     20   0  417768  30740  24888 S   0.0   0.2   0:00.08 xfce4-panel                                                                                        
    108 labex     20   0  340480  23232  18328 S   0.0   0.1   0:00.04 Thunar                                                                                             
    113 labex     20   0  473648  52032  34348 S   0.0   0.3   0:00.19 xfdesktop                                                                                          
    114 labex     20   0  339784  23920  19044 S   0.0   0.2   0:00.03 panel-6-systray                                                                                    
    137 labex     20   0  262944  18460  16200 S   0.0   0.1   0:00.02 xfce4-notifyd                                                                                      
labex:project/ $ pgrep bad_process.sh
609
labex:project/ $ kill 609
I refuse to terminate gracefully!                                                                                                                                         
labex:project/ $ kill -9 609
[1]  + 609 killed     ./bad_process.sh                                                                                                                                    
labex:project/ $  
```
![](Pasted%20image%2020261124153728.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab, i got the chance to demonstrate my understanding of the skills covered in this course. 