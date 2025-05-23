# Package Management in Linux

Linux me package management ka matlab hota hai software install, update, aur remove karna using package managers.

---

## Package Managers by Distribution

- **Debian/Ubuntu**: `apt`
- **RedHat/CentOS**: `yum` (old), `dnf` (new)
- **Arch Linux**: `pacman`

---

## 1. APT Commands (Debian/Ubuntu)

### Install a package:

```bash
sudo apt install <package-name>

Remove a package:

sudo apt remove <package-name>

Update package list:

sudo apt update

Upgrade installed packages:

sudo apt upgrade

Search for a package:

apt search <package-name>

Show package info:

apt show <package-name>


---

2. YUM/DNF Commands (RedHat/CentOS)

Install a package:

sudo yum install <package-name>
# OR
sudo dnf install <package-name>

Remove a package:

sudo yum remove <package-name>

Update all packages:

sudo yum update


---

3. Snap Packages (Ubuntu)

sudo snap install <package-name>
sudo snap remove <package-name>


---

4. Flatpak

Alternative universal package manager:

flatpak install <package-name>
flatpak run <package-name>


---

5. Verify Installed Package Version

apt list --installed | grep <package-name>


---

6. Clean Up

Remove unnecessary packages:

sudo apt autoremove


---

Important Notes

Root access usually required (sudo).

Commands may vary slightly across distributions.

Package managers also handle dependencies automatically.


---

