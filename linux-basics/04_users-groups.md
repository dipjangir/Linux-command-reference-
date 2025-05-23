# Users and Groups in Linux

## 1. Linux me Users kya hote hain?
Linux ek multi-user operating system hai — iska matlab hai ki ek hi system par kai users ek sath kaam kar sakte hain. Har user ka apna profile, permissions aur files hoti hain.

### Types of Users:
1. **Root User** – Sabse powerful user, jise sab kuch access hai.
2. **Normal User** – Limited permissions hoti hain. Apni files and applications access kar sakta hai.
3. **System Users** – System ke background processes ke liye hote hain (jaise `www-data`, `daemon`).

## 2. Groups kya hote hain?
Groups ka use kai users ko ek hi permissions dene ke liye hota hai. 

- **Primary Group**: Har user ka ek primary group hota hai.
- **Secondary Group**: User ek ya adhik secondary groups ka member ho sakta hai.

---

## 3. Important Commands:

| Command | Description |
|--------|-------------|
| `whoami` | Apna username dikhata hai |
| `id` | User ID (UID), Group ID (GID), aur group info dikhata hai |
| `groups` | User kis-kis group ka member hai wo dikhata hai |
| `adduser <username>` | Naya user create karta hai |
| `userdel <username>` | User delete karta hai |
| `groupadd <groupname>` | Naya group banata hai |
| `groupdel <groupname>` | Group delete karta hai |
| `usermod -aG <groupname> <username>` | User ko group me add karta hai |
| `passwd <username>` | User ka password set/change karta hai |

---

## 4. User & Group Information Files:

| File | Description |
|------|-------------|
| `/etc/passwd` | Users ki info hoti hai |
| `/etc/shadow` | Passwords ki encrypted info hoti hai |
| `/etc/group` | Groups ki info hoti hai |

---

## 5. Best Practices:
- Root user se direct kaam mat karo.
- Har user ke liye unique username use karo.
- Sensitive users ke liye strong passwords rakho.
- Groups ka sahi use karo permission manage karne ke liye.

---
