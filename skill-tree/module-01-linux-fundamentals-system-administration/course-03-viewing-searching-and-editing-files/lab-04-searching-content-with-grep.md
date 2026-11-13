# Lab: Searching Content with grep

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, we will be testing our ability to search content using the grep command.
- What problem were you tasked to solve?
1. Search for words.
2. Ignore capitalization (finding "Apple" when searching for "apple").
3. Filter out lines you _don't_ want to see.
---

## 🛠️ Commands & Configuration Used
```bash
cat (show whole file)
grep (search and print)
grep -i (search and print, ingore case)
grep -v (search and print, filter out)
```

---

## ✅ Results
- What was completed?
  I have learned the power of search.
1. **`grep "text" file`**: Finds the text.
2. **`grep -i`**: Finds text regardless of case.
3. **`grep -v`**: Hides lines containing the text.
- What output or verification confirmed success?
```shell
  
labex:project/ $ grep "root" /etc/passwd
root:x:0:0:root:/root:/bin/bash
labex:project/ $ cat ~/project/distros.txt
Ubuntu is user-friendly
UBUNTU is based on Debian
ubuntu uses GNOME
Fedora is cutting-edge
Arch is for power users
labex:project/ $ grep -i "ubuntu" ~/project/distros.txt
Ubuntu is user-friendly
UBUNTU is based on Debian
ubuntu uses GNOME
labex:project/ $ grep -v -i "ubuntu" ~/project/distros.txt
Fedora is cutting-edge
Arch is for power users
labex:project/ $ 

```
![](Pasted%20image%2020261113202430.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab i learned how to search for things in Linux, this is a very useful skill to have when i need to look for things I do not know where they are.