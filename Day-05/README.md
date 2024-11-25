# **Day 5: Loops (`for`, `while`) and `break`/`continue`**


## **What I Learned**
On Day 5, I learned:
- How to use `for` loops to iterate over sequences like lists, strings, and ranges.
- How to use `while` loops to repeatedly execute a block of code based on a condition.
- How to control loop behavior using `break` and `continue`.
- Nested loops for more complex iteration.


## **Key Concepts**

### **1. `for` Loops**
- `for` loops iterate over sequences such as lists, strings, and ranges.

**Example:**
```python
for num in range(1, 6):  # 1 to 5
    print(num)
```


### **2. `while` Loops**
- `while` loops continue as long as the condition is `True`.

**Example:**
```python
count = 5
while count > 0:
    print(count)
    count -= 1
print("Liftoff!")
```


### **3. `break` and `continue`**
- `break`: Exits the loop prematurely.
- `continue`: Skips the current iteration and proceeds to the next.

**Example:**
```python
for num in range(1, 10):
    if num == 5:
        break  # Exits the loop when num is 5
    if num % 2 == 0:
        continue  # Skips even numbers
    print(num)  # Prints odd numbers less than 5
```


### **4. Nested Loops**
- Loops inside loops are used for complex iterations.

**Example:**
```python
for i in range(1, 4):
    for j in range(1, 4):
        print(f"{i} x {j} = {i * j}")
    print("------")
```


## **Code Files**

### **1. `for_loop_examples.py`**
- Demonstrates basic `for` loops to iterate over lists, strings, and ranges.

### **2. `while_loop_examples.py`**
- Shows how `while` loops work with examples like countdowns.

### **3. `break_continue_examples.py`**
- Demonstrates the use of `break` and `continue` to control loop behavior.


## **Tasks**

### **Task 1: Multiplication Table**
Write a program to print the multiplication table for a given number.


**Solution:**
```python
num = int(input("Enter a number: "))

for i in range(1, 11):
    print(f"{num} x {i} = {num * i}")
```


### **Task 2: Guess the Number**
Write a program that:
1. Picks a random number between 1 and 100.
2. Allows the user to guess the number.
3. Provides feedback if the guess is too high or too low.


**Solution:**
```python
import random

number = random.randint(1, 100)
guess = None

while guess != number:
    guess = int(input("Guess the number (1-100): "))
    if guess < number:
        print("Too low!")
    elif guess > number:
        print("Too high!")
    else:
        print("Congratulations! You guessed it.")
```


### **Task 3: FizzBuzz**
Write a program to print numbers from 1 to 50, replacing:
- Multiples of 3 with "Fizz".
- Multiples of 5 with "Buzz".
- Multiples of both with "FizzBuzz".


**Solution:**
```python
for num in range(1, 51):
    if num % 3 == 0 and num % 5 == 0:
        print("FizzBuzz")
    elif num % 3 == 0:
        print("Fizz")
    elif num % 5 == 0:
        print("Buzz")
    else:
        print(num)
```


## **What's Next?**
On **Day 6**, I will explore **Lists and List Methods** in Python.
