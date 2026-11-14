# Lab: The PATH Variable

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the termina;, this lab will test our ability to use the path variable
- What problem were you tasked to solve?
  1. View your `PATH`.
  2. Use `which` to locate programs.
  3. Learn why executing local scripts requires `./`

---

## 🛠️ Commands & Configuration Used
```bash
$PATH (path of programs)
echo (print)
which (which program)
./ (this directory)
```

---

## ✅ Results
- What was completed?
   I have learned:
1. **The PATH is a map**: It is a list of folders where the system looks for programs.
2. **`which` locates programs**: It tells you exactly which file will be executed when you type a command.
3. **Safety First**: The current folder is not in the PATH by default. You must use `./` to run scripts you have just created or downloaded in your current location.
- What output or verification confirmed success?
```
labex:project/ $ echo $PATH
/usr/lib/jvm/java-11-openjdk-amd64/bin:/usr/lib/jvm/java-11-openjdk-amd64/bin:/usr/lib/jvm/java-11-openjdk-amd64/bin:/usr/lib/jvm/java-11-openjdk-amd64/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/home/labex/.local/bin:/usr/local/go/bin:/home/labex/golang/bin:/usr/share/maven/bin:/usr/local/bin:/usr/sbin/nodejs/bin:/usr/sbin/yarn/bin:/home/labex/.local/bin:/usr/local/go/bin:/home/labex/golang/bin:/usr/share/maven/bin:/usr/local/bin:/usr/sbin/nodejs/bin:/usr/sbin/yarn/bin
labex:project/ $ which date
/usr/bin/date
labex:project/ $ which ls
ls: aliased to ls --color=tty
labex:project/ $ which -a ls
ls: aliased to ls --color=tty
/usr/bin/ls
/bin/ls
labex:project/ $ ./hello.sh
Hello from the script!
labex:project/ $ 
```
![](Pasted%20image%2020261114145208.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
What I learned in this lab is how to use the path variable to determine where to locate a program and how to structure my prompt so that i can use a program in the current working directory.