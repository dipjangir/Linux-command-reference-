# Conditional Statements in Bash

Conditional statements ka use program ke flow ko decision-based banane ke liye hota hai.

---

## 1. if Statement

```bash
if [ condition ]
then
  # code
fi

Example:

num=10

if [ $num -gt 5 ]
then
  echo "$num is greater than 5"
fi


---

2. if-else Statement

if [ condition ]
then
  # true block
else
  # false block
fi

Example:

age=17

if [ $age -ge 18 ]
then
  echo "You are an adult"
else
  echo "You are a minor"
fi


---

3. if-elif-else Statement

if [ condition1 ]
then
  # block1
elif [ condition2 ]
then
  # block2
else
  # else block
fi

Example:

marks=75

if [ $marks -ge 90 ]
then
  echo "Grade A"
elif [ $marks -ge 60 ]
then
  echo "Grade B"
else
  echo "Grade C"
fi


---

4. Comparison Operators

Operator	Meaning

-eq	Equal to
-ne	Not equal to
-gt	Greater than
-lt	Less than
-ge	Greater or equal
-le	Less or equal



---

5. String Comparisons

if [ "$a" = "$b" ]       # equal
if [ "$a" != "$b" ]      # not equal
if [ -z "$a" ]           # is empty
if [ -n "$a" ]           # is not empty


---

6. File Condition Checks

if [ -f file.txt ]   # file exists
if [ -d dir ]        # directory exists
if [ -r file.txt ]   # readable
if [ -w file.txt ]   # writable
if [ -x file.txt ]   # executable


---

Pro Tip:

Always use double quotes in conditions: [ "$var" = "value" ]

Use [[ ... ]] for advanced pattern matching and safer syntax.



---

Example Script

#!/bin/bash

read -p "Enter a number: " num

if [ $num -gt 0 ]; then
  echo "Positive number"
elif [ $num -lt 0 ]; then
  echo "Negative number"
else
  echo "Zero"
fi

---
