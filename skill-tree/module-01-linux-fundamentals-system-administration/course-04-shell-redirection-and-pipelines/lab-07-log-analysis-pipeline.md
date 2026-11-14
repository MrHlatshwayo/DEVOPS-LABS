# Lab: Log Analysis Pipeline

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this we will be using the terminal, we will tested on our ability to analyze logs in the CLI
- What problem were you tasked to solve?
  **My Mission**:
1. **Count** frequency of requests per IP.
2. **Rank** the IPs by traffic volume.
3. **Save** a report.

---

## 🛠️ Commands & Configuration Used
```bash
cat (show file)
| (pipe)
sort (order content)
sort -n (order content numerically)
uniq -c (count duplicate)
```

---

## ✅ Results
- What was completed?
  In this challenge, I:
1. **Pipelined Data**: Connected tools with `|`.
2. **Pre-processed**: Used `sort` to prepare data.
3. **Analyzed**: Used `uniq -c` to count.
4. **Reported**: Used `sort -n` and `>` to finalize the report.
- What output or verification confirmed success?
```
  labex:project/ $ sort suspicious_ips.txt |uniq -c
     40 10.0.0.42
     15 10.0.0.5
     30 172.16.0.1
      1 192.168.1.102
      1 192.168.1.103
     50 192.168.1.105
      1 192.168.1.119
      1 192.168.1.126
      1 192.168.1.144
      1 192.168.1.164
     20 192.168.1.200
      1 192.168.1.206
      1 192.168.1.211
      1 192.168.1.213
      1 192.168.1.221
      1 192.168.1.227
      1 192.168.1.23
      1 192.168.1.233
      1 192.168.1.244
      1 192.168.1.251
      1 192.168.1.28
      1 192.168.1.66
      1 192.168.1.80
      1 192.168.1.84
      1 192.168.1.86
labex:project/ $ sort suspicious_ips.txt |uniq -c |sort -c > ip_report.txt
sort: -:2: disorder:      15 10.0.0.5
labex:project/ $ sort suspicious_ips.txt |uniq -c |sort -n > ip_report.txt
labex:project/ $ cat 
```
![](Pasted%20image%2020261114103344.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab we learned how to build a pipeline that sorts data, counts the duplicate data and orders it again in numerical order.