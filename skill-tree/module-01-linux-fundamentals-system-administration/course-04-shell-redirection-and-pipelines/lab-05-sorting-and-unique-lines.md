# Lab: Sorting and Unique Lines

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will test our ability sort data in Linux using the CLI
- What problem were you tasked to solve?
  In this lab, I will take a messy list, organize it, remove duplicates, and generate a summary report.

---

## 🛠️ Commands & Configuration Used
```bash
cat (show file)
sort (order file content)
uniq (remove duplicate content)
> (ouput to and replace)
```

---

## ✅ Results
- What was completed?
  In this lab, I learned how to organize and analyze text files using a two-step process:
1. **`sort`**: Groups identical lines together like organizing a deck of cards.
2. **`uniq`**: Filters out the duplicates from those groups.
- What output or verification confirmed success?
```
labex:project/ $ cat fruit.txt
apple
banana
apple
cherry
banana
date
apple
labex:project/ $ sort fruit.txt
apple
apple
apple
banana
banana
cherry
date
labex:project/ $ sort fruit.txt > sorted_fruit.txt
labex:project/ $ cat sorted_fruit.txt
apple
apple
apple
banana
banana
cherry
date
labex:project/ $ uniq sorted_fruit.txt
apple
banana
cherry
date
labex:project/ $ uniq sorted_fruit.txt > unique_fruit.txt
labex:project/ $ 
```
![](Pasted%20image%2020261114101629.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how to sort data and how to get rid of duplicate data found in sorted files.