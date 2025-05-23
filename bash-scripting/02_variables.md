# Variables in Bash

Bash me variables ka use data store karne ke liye hota hai. Variables dynamically typed hote hain.

---

## 1. Variable Declare Karna

```bash
name="DevOps"
age=25

No space allowed around =.

Values strings ho ya numbers, bash unhe as a string hi treat karta hai by default.



---

2. Variable Access Karna

echo $name
echo $age

Use $ to access value.


---

3. User Input Lena

read username
echo "Welcome, $username"

Ya

read -p "Enter your name: " username
echo "Hello, $username"


---

4. Default Value Dena

echo ${name:-"Guest"}

Agar name variable undefined hai to "Guest" print hoga.


---

5. Export Variable (Global banana)

export name="DevOps"

Exported variables child processes me bhi accessible hote hain.


---

6. Special Variables

Variable	Use

$0	Current script ka name
$1-$9	Positional parameters (args)
$#	Total arguments
$@	All arguments as separate words
$*	All arguments as single word
$$	Current script ka PID
$?	Last command ka exit status



---

Example

#!/bin/bash

name="DevOps Learner"
echo "Hello, $name"

read -p "Enter your city: " city
echo "You are from $city"


---

Best Practices

Double quotes zaroor lagao: "${var}" — word splitting se bachne ke liye.

Variable names meaningful rakho.


---
