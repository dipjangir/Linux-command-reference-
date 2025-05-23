# Bash Script Structure

Bash scripting Linux me automation ke liye bahut important hai. Har bash script ka basic structure hota hai:

---

## 1. Shebang (#!/bin/bash)

Script ke start me yeh line hoti hai jo interpreter batati hai:

```bash
#!/bin/bash

Iska matlab hai ki yeh script bash shell se run hogi.


---

2. Comments

Script me comments likhne ke liye # ka use hota hai:

# This is a comment


---

3. Commands

Aap normal Linux commands likh sakte ho:

echo "Hello, World!"


---

4. Variables

Script me variables define karne ke liye:

name="DevOps Learner"
echo "Hello, $name"


---

5. Executing a Script

Script ko execute karne ke 2 main tareeke hain:

Step 1: Script banana

nano myscript.sh

Step 2: Permission dena

chmod +x myscript.sh

Step 3: Run karna

./myscript.sh

Ya

bash myscript.sh


---

Sample Script

#!/bin/bash

# This is a sample script
name="DevOps Learner"
echo "Hello, $name"


---

Best Practices

Hamesha #!/bin/bash use karo.

Descriptive variable names lo.

Comments likho samjhane ke liye.

Error handling zarur karo (aage padhenge).


---
