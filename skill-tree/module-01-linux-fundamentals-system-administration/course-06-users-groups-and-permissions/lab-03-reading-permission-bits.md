# Lab: Reading Permission Bits

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will test our ability to read permissions.
- What problem were you tasked to solve?
  In this lab, I will decode strings like `-rw-r--r--` and numbers like `644`.

---

## 🛠️ Commands & Configuration Used
```bash
ls -l (list long format)
echo (print output)
```

---

## ✅ Results
- What was completed?
  You learned:
1. **The Structure**: `User` | `Group` | `Others`.
2. **The Symbols**: `r` (Read), `w` (Write), `x` (Execute).
3. **The Octal Math**:
    1. Read = 4
    2. Write = 2
    3. Execute = 1
- What output or verification confirmed success?
```
labex:project/ $ ls -l
total 0
-rw-r--r-- 1 labex labex 0 Nov 19 13:59 practice_file
labex:project/ $ echo "rw-" > user_perm.txt
labex:project/ $ echo "r--" > group_perm.txt
echo "r--" > others_perm.txt
labex:project/ $ echo "6
dquote> 
dquote> " > octal_value.txt
labex:project/ $ echo "644" > octal_value.txt
labex:project/ $ 
```
![](Pasted%20image%2020261119080750.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how to decode permissions using the octal value system.