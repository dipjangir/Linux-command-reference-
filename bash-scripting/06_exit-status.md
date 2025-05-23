# Bash Script Exit Status

Bash script ya command ka **exit status** batata hai ki wo successfully chali ya nahi.

- **0**  → Success (Command/script successfully run hua)
- **1–255** → Error (kuch issue ya failure hua)

---

## 1. Check Exit Status

Har command ke baad uska exit status `$?` se check kar sakte hain.

```bash
ls /home/user
echo $?  # Agar directory exist karti hai to 0, warna error code


---

2. Example:

#!/bin/bash

mkdir myfolder

if [ $? -eq 0 ]; then
  echo "Directory created successfully"
else
  echo "Failed to create directory"
fi


---

3. Script Exit Code

Script ke end me exit command se manually status return kar sakte ho.

#!/bin/bash

echo "Exiting with code 2"
exit 2


---

4. Usage in Conditional Statements

ping -c 1 google.com

if [ $? -ne 0 ]; then
  echo "Network issue"
else
  echo "Internet is working"
fi


---

5. Best Practices

Har critical command ke baad $? check karo

Scripts me appropriate exit codes use karo

Automation ya DevOps tools (like Jenkins, Ansible) exit status se hi samajhte hain ki script safal hui ya nahi


---

