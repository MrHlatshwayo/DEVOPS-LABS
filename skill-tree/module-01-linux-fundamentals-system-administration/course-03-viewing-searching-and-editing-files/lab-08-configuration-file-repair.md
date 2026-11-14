# Lab: Configuration File Repair

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we be using the terminal, it test us on a ability to configure file repairs using the CLI
- What problem were you tasked to solve?
  My mission:
1. **Confirm current settings**.
2. **Increase timeout** to prevent crashes.
3. **Enable logging** for debugging.

---

## 🛠️ Commands & Configuration Used
```bash
# Paste key commands or script snippets executed during the lab
```

---

## ✅ Results
- What was completed?
  
- What output or verification confirmed success?
```
labex:project/ $ grep "TIMEOUT" server/comfig/app.conf
grep: server/comfig/app.conf: No such file or directory
labex:project/ $ grep "TIMEOUT" server/config/app.conf
TIMEOUT=5
labex:project/ $ vim server/config/app.conf
labex:project/ $ vim server/config/app.conf
labex:project/ $ cat server/config/app.conf
# Server Configuration File
# Created by: SysAdmin Team

PORT=8080
HOST=0.0.0.0
TIMEOUT=30
MAX_CONNECTIONS=100
DB_HOST=localhost
ENABLE_LOGGING=yes
labex:project/ $ 

```
![](Pasted%20image%2020261114093353.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
