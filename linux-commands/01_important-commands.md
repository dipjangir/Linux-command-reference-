# Important Linux Commands for Cloud/DevOps Beginners

Ye kuch commonly used Linux commands hain jo Cloud/DevOps work ke liye frequently use hote hain.

---

## 1. System Information

| Command | Description |
|---------|-------------|
| `uname -a` | System information (kernel version, OS, etc.) |
| `hostname` | System ka hostname |
| `uptime` | System kitne time se chalu hai |

---

## 2. File & Directory Management

| Command | Description |
|---------|-------------|
| `ls` | Directory listing |
| `ls -l` | Long listing format |
| `ls -a` | Hidden files bhi dikhata hai |
| `cd <dir>` | Directory change karta hai |
| `pwd` | Current directory ka path |
| `mkdir <dir>` | Nayi directory banata hai |
| `rm <file>` | File delete karta hai |
| `rm -r <dir>` | Directory with contents delete karta hai |
| `cp <src> <dest>` | Copy file ya folder |
| `mv <src> <dest>` | Move ya rename karta hai |
| `touch <file>` | Nayi empty file create karta hai |

---

## 3. File Viewing

| Command | Description |
|---------|-------------|
| `cat <file>` | File content dikhata hai |
| `more <file>` | File ko page by page dikhata hai |
| `less <file>` | Advanced file viewer |
| `head <file>` | File ke top 10 lines |
| `tail <file>` | File ke last 10 lines |

---

## 4. File Permissions & Ownership

| Command | Description |
|---------|-------------|
| `chmod` | File permissions change karta hai |
| `chown` | Ownership change karta hai |
| `ls -l` | Permissions aur owner dikhata hai |

---

## 5. Process Management

| Command | Description |
|---------|-------------|
| `ps` | Running processes |
| `top` | Real-time process monitoring |
| `kill <PID>` | Process terminate karta hai |
| `htop` | Advanced interactive process viewer (if installed) |

---

## 6. Networking Commands

| Command | Description |
|---------|-------------|
| `ping <host>` | Host reachable hai ya nahi check karta hai |
| `ifconfig` / `ip a` | Network interface details |
| `netstat -tulnp` | Listening ports |
| `curl <url>` | Web request bhejna |
| `wget <url>` | File download karna |

---

## 7. Package Management (Ubuntu/Debian)

| Command | Description |
|---------|-------------|
| `sudo apt update` | Package list update karta hai |
| `sudo apt upgrade` | All packages upgrade karta hai |
| `sudo apt install <pkg>` | Naya package install karta hai |
| `sudo apt remove <pkg>` | Package remove karta hai |

---

## 8. System Monitoring

| Command | Description |
|---------|-------------|
| `df -h` | Disk usage |
| `du -sh <dir>` | Directory size |
| `free -h` | Memory usage |
| `top` / `htop` | Live process view |

---

## 9. User Management

| Command | Description |
|---------|-------------|
| `adduser <username>` | Naya user banata hai |
| `passwd <username>` | Password set/change karta hai |
| `usermod -aG <group> <user>` | Group me add karta hai |

---

## 10. Help & Documentation

| Command | Description |
|---------|-------------|
| `man <command>` | Manual page dikhata hai |
| `--help` | Command ka short help |

---

**Note:** Ye commands basic practice ke liye kaafi important hain. Inka use daily basis pe hota hai especially jab servers ya automation scripts handle karte ho.
