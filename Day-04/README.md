# **Day 4: Conditionals (`if`, `else`, `elif`)**


## **What I Learned**
On Day 4, I focused on:
- Writing conditional statements (`if`, `else`, `elif`) to control program flow.
- Using logical operators (`and`, `or`, `not`) to handle complex conditions.
- Implementing nested conditionals for multi-level decision-making.


## **Key Concepts**

### **1. Conditional Statements**
- **`if`:** Executes a block of code if the condition is `True`.
- **`else`:** Executes a block of code if the condition in `if` is `False`.
- **`elif`:** Used to check multiple conditions sequentially.

**Example:**
```python
marks = 85
if marks >= 90:
    print("Grade: A+")
elif marks >= 75:
    print("Grade: A")
else:
    print("Grade: B")
```


### **2. Logical Operators**
Logical operators are used to combine multiple conditions:
- **`and`:** All conditions must be `True`.
- **`or`:** At least one condition must be `True`.
- **`not`:** Negates a condition.

**Examples:**
```python
age = 20
is_registered = True

if age >= 18 and is_registered:
    print("You can vote.")

if not is_registered:
    print("Please register to vote.")
```


### **3. Nested Conditionals**
You can nest `if` statements for complex decision-making.

**Example:**
```python
age = 20
if age >= 18:
    if age < 21:
        print("Eligible to vote but not drink alcohol in the US.")
    else:
        print("Eligible for both.")
else:
    print("Not eligible to vote.")
```


## **Code Examples**

### **Example 1: Check Even or Odd**
```python
num = int(input("Enter a number: "))

if num % 2 == 0:
    print(f"{num} is an even number.")
else:
    print(f"{num} is an odd number.")
```


### **Example 2: Grading System**
```python
marks = int(input("Enter your marks: "))

if marks >= 90:
    print("Grade: A+")
elif marks >= 75:
    print("Grade: A")
elif marks >= 50:
    print("Grade: B")
else:
    print("Grade: F")
```


### **Example 3: Determine Age Group**
```python
age = int(input("Enter your age: "))

if age < 13:
    print("You are a child.")
elif age < 18:
    print("You are a teenager.")
else:
    print("You are an adult.")
```


## **Tasks**

### **Task 1: Temperature Checker**
Write a program that:
1. Takes a temperature value as input.
2. Displays whether it's **hot**, **warm**, or **cold**.

**Solution:**
```python
temp = int(input("Enter the temperature: "))

if temp >= 30:
    print("It's hot!")
elif temp >= 20:
    print("It's warm.")
else:
    print("It's cold.")
```


### **Task 2: Leap Year Checker**
Write a program to check whether a given year is a leap year.

**Solution:**
```python
year = int(input("Enter a year: "))

if year % 4 == 0:
    if year % 100 != 0 or year % 400 == 0:
        print(f"{year} is a leap year.")
    else:
        print(f"{year} is not a leap year.")
else:
    print(f"{year} is not a leap year.")
```


### **Task 3: Simple Calculator**
Write a program to take two numbers and an operator (`+`, `-`, `*`, `/`) as input and perform the corresponding calculation.

**Solution:**
```python
num1 = float(input("Enter the first number: "))
num2 = float(input("Enter the second number: "))
operator = input("Enter an operator (+, -, *, /): ")

if operator == "+":
    print(f"The result is: {num1 + num2}")
elif operator == "-":
    print(f"The result is: {num1 - num2}")
elif operator == "*":
    print(f"The result is: {num1 * num2}")
elif operator == "/":
    if num2 != 0:
        print(f"The result is: {num1 / num2}")
    else:
        print("Error: Division by zero!")
else:
    print("Invalid operator.")
```

## **What's Next?**
Next, I will explore **Day 5: Loops (`for`, `while`, `break`, `continue`)**.
