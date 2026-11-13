# Lab: Filesystem Cleanup Task

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, this lab will test everything we have learned in this course.
- What problem were you tasked to solve?
  1. **Create a directory structure** to categorize files.
  2. **Secure critical data** by creating a backup.
  3. **Sort files** into their respective folders.
  4. **Clean up** unnecessary temporary files.

---

## 🛠️ Commands & Configuration Used
```bash
ls (list)
cd (change directory)
rm (remove)
* (wildcard)
mkdir (make directory)
mv (rename/move)
```

---

## ✅ Results
- What was completed?
  In this challenge, I demonstrated essential skills:
1. **Organization**: Using `mkdir` to create structure.
2. **Safety**: Using `cp` to backup data.
3. **Categorization**: Using `mv` and wildcards to sort files.
4. **Hygiene**: Using `rm` to clear junk.
- What output or verification confirmed success?
```
labex:project/ $ ls
workspace
labex:project/ $ cd workspace
labex:workspace/ $ mkdir images docs backups
labex:workspace/ $ ls
backups  banner.jpg  cache.tmp  docs  error.tmp  images  logo.jpg  notes.txt  profile.jpg  readme.txt  session.tmp  todo.txt
labex:workspace/ $ cp readme.txt backups/
labex:workspace/ $ ls backups
readme.txt
labex:workspace/ $ ls *.jpg
banner.jpg  logo.jpg  profile.jpg
labex:workspace/ $ mv *.jpg images/
labex:workspace/ $ ls images
banner.jpg  logo.jpg  profile.jpg
labex:workspace/ $ ls
backups  cache.tmp  docs  error.tmp  images  notes.txt  readme.txt  session.tmp  todo.txt
labex:workspace/ $ ls
backups  cache.tmp  docs  error.tmp  images  notes.txt  readme.txt  session.tmp  todo.txt
labex:workspace/ $ mv *.txt docs/
labex:workspace/ $ ls docs/
notes.txt  readme.txt  todo.txt
labex:workspace/ $ ls
backups  cache.tmp  docs  error.tmp  images  session.tmp
labex:workspace/ $ rm *.tmp
labex:workspace/ $ ls
backups  docs  images
labex:workspace/ $ 
```
![](Pasted%20image%2020261113194312.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
In this lab I was tested on my ability to use all the commands taught in this course. I did not encounter any errors but i was really relived to have gotten some practice.