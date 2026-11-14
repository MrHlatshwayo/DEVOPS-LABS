# Lab: Standard Input, Output, and Error

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, we will be tested on our knowledge of inputs, outputs and errors.
- What problem were you tasked to solve?
1. **Standard Output (stdout)**: The "Good Chute". When the machine works correctly, the finished product comes out here.
2. **Standard Error (stderr)**: The "Bad Chute". If something goes wrong, error messages come out here.
---

## 🛠️ Commands & Configuration Used
```bash
ls -l (list long format)
```

---

## ✅ Results
- What was completed?
  In this lab, I explored "Data Streams" using the two-chute machine analogy:
1. **Standard Output**: The channel for normal results.
2. **Standard Error**: The channel for error messages.
- What output or verification confirmed success?
```
labex:project/ $ ls -l
total 0
-rw-rw-r-- 1 labex labex 0 Nov 14 15:35 file1.txt
-rw-rw-r-- 1 labex labex 0 Nov 14 15:35 file2.txt
labex:project/ $ ls -l /nonexistent_directory
ls: cannot access '/nonexistent_directory': No such file or directory
labex:project/ $ ls -l . /fake
ls: cannot access '/fake': No such file or directory
.:
total 0
-rw-rw-r-- 1 labex labex 0 Nov 14 15:35 file1.txt
-rw-rw-r-- 1 labex labex 0 Nov 14 15:35 file2.txt
labex:project/ $  
```
![](Pasted%20image%2020261114094154.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how Linux process the output of command in two streams and how it is able to print them out separatelty than mixing them.