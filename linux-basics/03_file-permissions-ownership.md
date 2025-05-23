# Linux File Permissions & Ownership

Linux me har file aur directory ke saath **permissions aur ownership** set hoti hai, jo batati hai ki kaun kya access kar sakta hai.

---

## 1. Ownership Types:

Har file ke 3 owner hote hain:

- **User (u)**: File ka owner (creator)
- **Group (g)**: Ek group of users
- **Others (o)**: Baaki sab users (na user na group)

---

## 2. Permission Types:

Har owner ke liye 3 tarah ki permissions hoti hain:

| Permission | Symbol | Meaning               |
|------------|--------|------------------------|
| Read       | `r`    | File padna ya dir me dekhna |
| Write      | `w`    | File me changes ya dir me naye file create/delete |
| Execute    | `x`    | File execute ya dir access (cd) karna |

---

## 3. ls -l Output samajhna:

```bash
ls -l file.txt
Output: -rwxr-xr-- 1 user group 1234 May 13 10:00 file.txt
Field	/ Meaning

-	File type (file = -, dir = d)
rwx	User permissions
r-x	Group permissions
r--	Others permissions
user	File ka owner
group	Owner group
1234	File size in bytes
May 13	Modified date

