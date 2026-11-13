# Lab: Determining File Types

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, this lab will test our ability to determine file types in Linux using the CLI
- What problem were you tasked to solve?
  In this lab, I will use the `file` command to specific the true nature of files, regardless of what they are named.

---

## 🛠️ Commands & Configuration Used
```shell
ls (list)
cat (concatenate)
file (file content/type)
```

---

## ✅ Results
- What was completed?
  I have learned to look past the label and see the true nature of files.
1. **`file filename`**: The command to uncover the truth.
2. **Extensions lie**: `.jpg` doesn't always mean image.
3. **No extension? No problem**: Linux doesn't need extensions to know what a file is.
- What output or verification confirmed success?
```shell
labex:project/ $ ls -l
total 12
-rw-rw-r-- 1 labex labex 46 Nov 14 02:06 fake_image.jpg
-rw-rw-r-- 1 labex labex 70 Nov 14 02:06 mystery_file
-rw-rw-r-- 1 labex labex 36 Nov 14 02:06 welcome.txt
labex:project/ $ file welcome.txt
welcome.txt: ASCII text
labex:project/ $ file /bin/ls
/bin/ls: ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, BuildID[sha1]=36b86f957a1be53733633d184c3a3354f3fc7b12, for GNU/Linux 3.2.0, stripped
labex:project/ $ file mystery_file
mystery_file: PNG image data, 1 x 1, 8-bit/color RGBA, non-interlaced
labex:project/ $ file fake_image.jpg
fake_image.jpg: ASCII text
labex:project/ $ cat fake_image.jpg
This is actually just text, not a JPEG image.
labex:project/ $ 
```
![](Pasted%20image%2020261113201350.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I learned how extensions can be deceiving, from a security perspective this is very command to know when dealing with new systems or files or unkown origin,  