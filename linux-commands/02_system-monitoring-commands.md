# System Monitoring Commands in Linux

System ki performance aur health monitor karne ke liye ye commands bahut useful hain. Cloud/DevOps me inka use frequently hota hai.

---

## 1. `top`

- Real-time me running processes show karta hai.
- CPU, memory usage, PID, user, etc. ka detail view deta hai.

```bash
top
2. htop

top ka interactive version hai (pehle install karna padta hai).

Process ko kill ya sort karna easy hota hai.


sudo apt install htop
htop


---

3. ps

Static snapshot deta hai running processes ka.

Example:


ps aux


---

4. free

RAM aur swap memory ka use dikhata hai.


free -h


---

5. vmstat

System performance ka summary deta hai (CPU, memory, IO, etc.).


vmstat 1 5


---

6. iostat

CPU aur disk IO activity ka data deta hai.


sudo apt install sysstat
iostat


---

7. df

File system disk space usage dikhata hai.


df -h


---

8. du

Directory ya file ka space usage batata hai.


du -sh /path/to/directory


---

9. uptime

System kitne time se chalu hai aur load average kya hai, ye dikhata hai.


uptime


---

10. sar

Historic system performance monitor karta hai.

sysstat package se install hota hai.


sudo apt install sysstat
sar -u 1 3


---

11. netstat / ss

Network connections, listening ports, routing tables dikhata hai.


netstat -tulnp
ss -tulnp


---

12. top + 1

CPU cores ka individual usage dikhata hai.


top
# Press '1' key inside top


---

13. watch

Kisi bhi command ko interval pe repeat karta hai.


watch -n 2 free -h


---

Note: Ye commands system monitoring aur troubleshooting me bahut kaam aati hain, specially jab kisi server ka performance issue check karna hota hai.

---
