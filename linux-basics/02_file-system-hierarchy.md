# Linux File System Hierarchy

Linux ka file system ek tree-like structure hota hai jisme sab kuch **root (`/`) directory** se start hota hai.

---

## Important Directories:

| Directory  | Description |
|------------|-------------|
| `/`        | Root directory - sab kuch yahi se start hota hai |
| `/bin`     | System ke basic executable commands (jaise `ls`, `cp`, `mv`) |
| `/sbin`    | System binaries for admin (jaise `shutdown`, `reboot`) |
| `/etc`     | Configuration files (jaise `/etc/hosts`, `/etc/passwd`) |
| `/home`    | Users ke personal folders (jaise `/home/user1`) |
| `/root`    | Root (admin) user ka personal directory |
| `/var`     | Variable files - logs, spool, etc. |
| `/tmp`     | Temporary files (boot ke baad clean ho jate hain) |
| `/usr`     | User-related programs aur libraries |
| `/lib`     | System libraries (shared files `.so`) |
| `/boot`    | Boot-related files (like kernel, grub) |
| `/dev`     | System devices (jaise `/dev/sda` - hard disk) |
| `/mnt`     | Manually mounted filesystems |
| `/proc`    | System process info (virtual) |
| `/sys`     | System hardware info (virtual) |

---

## Visual Structure:/ ├── bin/ ├── boot/ ├── dev/ ├── etc/ ├── home/ │   └── user/ ├── lib/ ├── media/ ├── mnt/ ├── opt/ ├── proc/ ├── root/ ├── sbin/ ├── tmp/ ├── usr/ └── var/
---

## Notes:
- Linux me **sab kuch file hota hai** (even devices & processes).
- Hierarchy samajhna zaruri hai taaki file navigate, troubleshoot aur configure karna easy ho.
