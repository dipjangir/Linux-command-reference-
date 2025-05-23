# Loops in Bash

Loops se hum kisi bhi task ko repeatedly execute kara sakte hain jab tak koi condition true ho.

---

## 1. while Loop

```bash
while [ condition ]
do
  # code block
done

Example:

count=1
while [ $count -le 5 ]
do
  echo "Count: $count"
  ((count++))
done


---

2. until Loop

until [ condition ]
do
  # code block
done

Example:

count=1
until [ $count -gt 5 ]
do
  echo "Count: $count"
  ((count++))
done


---

3. for Loop

for var in list
do
  # code block
done

Example:

for i in 1 2 3 4 5
do
  echo "Number: $i"
done


---

4. C-style for Loop (Bash 3+)

for (( i=0; i<5; i++ ))
do
  echo $i
done


---

5. Loop with Break and Continue

break:

Loop ko turant terminate kar deta hai.

for i in 1 2 3 4 5
do
  if [ $i -eq 3 ]
  then
    break
  fi
  echo "Number: $i"
done

continue:

Current iteration skip karta hai, loop next pe chala jata hai.

for i in 1 2 3 4 5
do
  if [ $i -eq 3 ]
  then
    continue
  fi
  echo "Number: $i"
done


---

Loop Through Files

for file in *.txt
do
  echo "Processing $file"
done


---

Loop Through Command Output

for user in $(cat users.txt)
do
  echo "User: $user"
done


---

Tip:

Avoid infinite loops accidentally: Always include condition update in loop.

Use do ... done carefully with spacing.


---

