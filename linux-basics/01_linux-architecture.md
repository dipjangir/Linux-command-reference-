Linux Architecture Notes 
# Linux Architecture

Linux ek open-source operating system hai jo mainly 3 main layers me divided hota hai:

---

## 1. **Kernel**:
- Ye Linux ka core part hota hai.
- Hardware aur software ke beech bridge ka kaam karta hai.
- Process management, memory, device control sab yahi handle karta hai.

### Types of Kernel:
- **Monolithic Kernel**: Linux ka kernel monolithic hota hai, jisme saari services ek hi large block me hoti hain.

---

## 2. **System Libraries**:
- Ye wo libraries hoti hain jo OS ke functionalities ko access karne ke liye apps ko help karti hain.
- Jaise: glibc (GNU C Library)

---

## 3. **System Utilities**:
- Inka kaam user ko system operate karne me madad dena hai.
- Example: `cp`, `mv`, `mkdir`, `ls` — ye sab system utilities ke example hain.

---

## Diagram (Conceptual):
+-----------------------+ |  Applications         | +-----------------------+ |  System Utilities     | +-----------------------+ |  System Libraries     | +-----------------------+ |      Kernel           | +-----------------------+ |      Hardware         | +-----------------------+
---

## Summary:
- Linux me har cheez ek hierarchy ke form me kaam karti hai.
- Sabse neeche hardware, upar kernel, phir libraries, aur finally user level utilities aur applications.
