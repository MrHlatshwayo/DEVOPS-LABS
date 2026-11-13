# Lab: Using Wildcards and Globbing

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, this lab tests us on our ability to use wildcards and globbing 
- What problem were you tasked to solve?
  In this lab, I will learn two powerful symbols:
1. The **Asterisk (`*`)**: Represents _anything_ (any length).
2. The **Question Mark (`?`)**: Represents _one single character_.

---

## 🛠️ Commands & Configuration Used
```bash
ls (list)
rm (remove)
mv (rename/move)
* (wildcard)
? (single character)
```

---

## ✅ Results
- What was completed?
  I have learned the power of pattern matching.
- **`*` (Asterisk)**: The "Match Everything" wildcard. Great for selecting all files of a type (`*.png`) or all files in a series (`day_*`).
- **`?` (Question Mark)**: The "Single Character" wildcard. Great for precise matching (`file_?.txt`).
- What output or verification confirmed success?
```
labex:project/ $ ls
data_2024.csv  data_2025.csv  data_old.log  image.png  notes.txt  readme.txt  report.txt  script.py  temp_1  temp_2  temp_a
labex:project/ $ ls *.txt
notes.txt  readme.txt  report.txt
labex:project/ $ mkdir backup
labex:project/ $ mv data_* backup/
labex:project/ $ ls
backup  image.png  notes.txt  readme.txt  report.txt  script.py  temp_1  temp_2  temp_a
labex:project/ $ ls backup
data_2024.csv  data_2025.csv  data_old.log
labex:project/ $ ls temp_?
temp_1  temp_2  temp_a
labex:project/ $ rm temp_?
labex:project/ $ ls
backup  image.png  notes.txt  readme.txt  report.txt  script.py
labex:project/ $ 

```
![](Pasted%20image%2020261113193210.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
What I learned in this lab is how to use * and ? for pattern matching when i remove or move files. This is very convenient when i need to utilize multiple files at once.