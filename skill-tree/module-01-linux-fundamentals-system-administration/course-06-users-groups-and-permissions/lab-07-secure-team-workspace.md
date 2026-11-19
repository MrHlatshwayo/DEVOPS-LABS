# Lab: Secure Team Workspace

## 🎯 Lab Objectives
- What specific skill or tool was tested?
  In this lab we will be using the terminal, it will be testing our ability to secure a team workspace.
- What problem were you tasked to solve?
  **Your Mission**:
1. **Verify** Alice's account and group.
2. **Create** a shared workspace `/srv/dev`.
3. **Secure** it so only developers can access it.

---

## 🛠️ Commands & Configuration Used
```bash
id (user info)
sudo (root privelege)
mkdir 
chmod
chgrp
```

---

## ✅ Results
- What was completed?
  In this challenge, you:
1. **Audited Users**: Verified account setup.
2. **Created Structure**: Built `/srv/dev`.
3. **Managed Ownership**: Assigned group ownership.
4. **Secured Permissions**: Used `chmod 770` to block strangers.
- What output or verification confirmed success?
```
labex:project/ $ id alice
uid=5001(alice) gid=5001(alice) groups=5001(alice),5003(developers)
labex:project/ $ sudo mkdir /srv/dev
labex:project/ $ cd /srv/dev
labex:dev/ $ sudo chgrp developers /srv/dev
labex:dev/ $ sudo chmod 770 /srv/dev
labex:dev/ $ 
```
![](Pasted%20image%2020261119091257.png)
---

## 📝 Notes
- Lessons learned, troubleshooting steps, or follow-up work.
