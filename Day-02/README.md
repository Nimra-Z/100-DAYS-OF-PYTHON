## **Day 2: Variables, Data Types, and Type Casting**

## **What I Learned**
Today, I learned:
- How to declare and use variables in Python.
- The different data types in Python (`int`, `float`, `str`, `bool`, etc.).
- How to convert one data type into another using **type casting**.
- How to take user input with the `input()` function and process it.


## **Key Concepts**

### **1. Variables**
- Variables are used to store data in Python.
- Python automatically determines the type of a variable based on the value assigned.

**Example:**
```python
name = "Alice"          # String
age = 25                # Integer
height = 5.5            # Float
is_student = True       # Boolean
```


### **2. Data Types**
Python supports various data types. Here are the commonly used ones:

| **Type**    | **Description**           | **Example**               |
|-------------|---------------------------|---------------------------|
| `int`       | Integer (whole number)    | `age = 25`               |
| `float`     | Floating-point number     | `height = 5.5`           |
| `str`       | String (text)             | `name = "Alice"`         |
| `bool`      | Boolean (True/False)      | `is_student = True`      |
| `list`      | Ordered, mutable sequence | `fruits = ["apple"]`     |
| `tuple`     | Ordered, immutable sequence | `point = (1, 2)`      |
| `set`       | Unordered collection of unique items | `colors = {"red"}` |
| `dict`      | Key-value pairs           | `person = {"name": "Alice"}` |


### **3. Type Casting**
Type casting is used to convert variables from one type to another.

**Examples:**
```python
# String to Integer
num_str = "123"
num_int = int(num_str)

# Integer to Float
num_float = float(num_int)

# Float to String
price = 19.99
price_str = str(price)
```


### **4. Taking User Input**
Use the `input()` function to take input from the user. Input is always stored as a string.

**Example:**
```python
name = input("Enter your name: ")
age = int(input("Enter your age: "))
print(f"Hello, {name}. You are {age} years old.")
```


## **Code Examples**

### **Example 1: Working with Variables**
```python
name = "Alice"
age = 25
height = 5.5
is_student = True

print("Name:", name)
print("Age:", age)
print("Height:", height)
print("Is Student:", is_student)
```


### **Example 2: Type Casting**
```python
num_str = "123"
num_int = int(num_str)
num_float = float(num_int)

print("String to Integer:", num_int)
print("Integer to Float:", num_float)
```


### **Example 3: User Input**
```python
name = input("Enter your name: ")
age = int(input("Enter your age: "))
print(f"Hello {name}, you are {age} years old.")
```


## **Tasks**

### **Task 1: Add Two Numbers**
Write a program that:
1. Takes two numbers as input from the user.
2. Converts the inputs to integers.
3. Performs addition and displays the result.

**Solution:**
```python
num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))
sum_result = num1 + num2
print("The sum is:", sum_result)
```


### **Task 2: Greeting with Name and Age**
Write a program that:
1. Asks for a user's name and age.
2. Outputs a personalized message.

**Solution:**
```python
name = input("What is your name? ")
age = int(input("How old are you? "))
print(f"Hello, {name}! Next year, you will be {age + 1} years old.")
```

## **What's Next?**
On **Day 3**, we will dive into **Conditionals (`if`, `else`, `elif`) and Logical Operators**.
