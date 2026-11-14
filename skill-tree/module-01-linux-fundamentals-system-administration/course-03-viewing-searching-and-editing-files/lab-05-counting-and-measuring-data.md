# Lab: Counting and Measuring Data

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, this lab will test our ability to count and measure data using the CLI
- What problem were you tasked to solve?
  In this lab, I will use `wc` to answer three questions:
   "How long is it?", "How many words?", and "How big is it?"
---

## 🛠️ Commands & Configuration Used
```bash
cat (show whole file)
wc (word count/measure)
wc -l (count lines)
wc -w (count words)
wc -c (count bytes)
```

---

## ✅ Results
- What was completed?
  I have learned to use the Linux accountant, `wc`.
1. **`wc -l`**: Count lines (records).
2. **`wc -w`**: Count words.
3. **`wc -c`**: Count size/bytes.
- What output or verification confirmed success?
```
labex:project/ $ cat sample.txt
Linux is an open-source operating system.
It is widely used for servers and development.
The command line interface is powerful.
Learning Linux commands is fun.
labex:project/ $ wc -l sample.txt
4 sample.txt
labex:project/ $ wc -l sample.txt > lines.txt 
labex:project/ $ wc -w sample.txt
25 sample.txt
labex:project/ $ wc -w sample.tx > words.txt
wc: sample.tx: No such file or directory
labex:project/ $ wc -w sample.txt > words.txt
labex:project/ $ wc -c sample.txt
161 sample.txt
labex:project/ $ wc -c sample.txt > bytes.txt
labex:project/ $ 
```
![](Pasted%20image%2020261114091036.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how to measure data namely lines, words and characters/bytes inside of files.