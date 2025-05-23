# Bash Functions

Functions ka use repeat hone wale code ko ek jagah define karne ke liye hota hai. Isse code reusable aur clean banta hai.

---

## 1. Function Define Karna

### Syntax 1:
```bash
function function_name {
  # commands
}

Syntax 2:

function_name() {
  # commands
}


---

2. Function Call Karna

Function ko sirf naam likh kar call karte hain:

greet_user


---

3. Example:

greet_user() {
  echo "Hello, User!"
}

greet_user


---

4. Function with Parameters

print_sum() {
  echo "Sum is: $(($1 + $2))"
}

print_sum 5 10

$1, $2 ... are positional parameters.



---

5. Returning Values

return command exit status (0–255) return karta hai. Value return karne ke liye echo use karte hain.

get_name() {
  echo "ChatGPT"
}

username=$(get_name)
echo "User: $username"


---

6. Scope of Variables

By default, variables globally accessible hoti hain. Local variable define karne ke liye local keyword use karo.

my_function() {
  local var="I am local"
  echo $var
}


---

7. Recursive Function

Function jo khud ko call karta hai.

factorial() {
  if [ $1 -le 1 ]; then
    echo 1
  else
    prev=$(factorial $(($1 - 1)))
    echo $(($1 * $prev))
  fi
}

factorial 5


---

Best Practices

Function naam meaningful hona chahiye

Function ke andar error handle karo

Reusability aur modular design maintain karo


---
# Bash Functions

Functions ka use repeat hone wale code ko ek jagah define karne ke liye hota hai. Isse code reusable aur clean banta hai.

---

## 1. Function Define Karna

### Syntax 1:
```bash
function function_name {
  # commands
}

Syntax 2:

function_name() {
  # commands
}


---

2. Function Call Karna

Function ko sirf naam likh kar call karte hain:

greet_user


---

3. Example:

greet_user() {
  echo "Hello, User!"
}

greet_user


---

4. Function with Parameters

print_sum() {
  echo "Sum is: $(($1 + $2))"
}

print_sum 5 10

$1, $2 ... are positional parameters.



---

5. Returning Values

return command exit status (0–255) return karta hai. Value return karne ke liye echo use karte hain.

get_name() {
  echo "ChatGPT"
}

username=$(get_name)
echo "User: $username"


---

6. Scope of Variables

By default, variables globally accessible hoti hain. Local variable define karne ke liye local keyword use karo.

my_function() {
  local var="I am local"
  echo $var
}


---

7. Recursive Function

Function jo khud ko call karta hai.

factorial() {
  if [ $1 -le 1 ]; then
    echo 1
  else
    prev=$(factorial $(($1 - 1)))
    echo $(($1 * $prev))
  fi
}

factorial 5


---

Best Practices

Function naam meaningful hona chahiye

Function ke andar error handle karo

Reusability aur modular design maintain karo


---
