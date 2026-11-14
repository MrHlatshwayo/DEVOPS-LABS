# Lab: Redirection to Files

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, It will test our ability to redirect files.
- What problem were you tasked to solve?
  In this lab, I will learn three ways to control where data goes:
1. **Redirect and Overwrite (`>`)**: Saves output to a file, replacing unmatched content.
2. **Redirect and Append (`>>`)**: Adds output to the end of a file.
3. **Error Redirection (`2>`)**: Catches error messages only.

---

## 🛠️ Commands & Configuration Used
```bash
> (output to and replace)
>> (output to and ammend)
2> (output error to)
```

---

## ✅ Results
- What was completed?
  I have mastered the art of traffic control:
- **`>` (Overwrite)**: Saves output to a file (wipes previous content).
- **`>>` (Append)**: Adds output to end of file (keeps history).
- **`2>` (Error Redirect)**: Catches error messages.
- What output or verification confirmed success?
```
labex:project/ $ echo "Hello, Linux." > output.txt
labex:project/ $ cat output.txt
Hello, Linux.
labex:project/ $ echo "This is new content." > output.txt
cat output.txt
This is new content.
labex:project/ $ echo "This line is appended." >> output.txt
cat output.txt
This is new content.
This line is appended.
labex:project/ $ echo "Another line." >> output.txt
cat output.txt
This is new content.
This line is appended.
Another line.
labex:project/ $ ls /missing_directory 2> error.log
labex:project/ $ cat error.log
ls: cannot access '/missing_directory': No such file or directory
labex:project/ $ 
```
![](Pasted%20image%2020261114094928.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how redirect messages to certain files, including errors to error logs.