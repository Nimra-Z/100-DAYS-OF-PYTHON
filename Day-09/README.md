# **Day 9: Defining Functions, Arguments, and Return Values**

Welcome to **Day 9** of the **100 Days of Python** journey! 🎉 Today, we dive into one of the most fundamental concepts in Python — **functions**. Functions allow us to write clean, reusable, and modular code, making programs easier to maintain and debug.


## **What You’ll Learn Today**

### **Key Concepts**
1. **Defining Functions**:
   - Use the `def` keyword to define a function.
   - Write reusable blocks of code that can be called multiple times.

2. **Function Arguments**:
   - Understand how to pass data into functions using parameters.
   - Differentiate between positional and keyword arguments.

3. **Return Values**:
   - Use `return` to send data back to the caller.
   - Understand the importance of return values in building modular code.

4. **Default Parameters**:
   - Learn how to set default values for arguments.

5. **Positional vs Keyword Arguments**:
   - Discover the flexibility of passing arguments by position or name.


## **Folder Structure**

```plaintext
Day_9_Defining_Functions
├── examples
│   ├── basic_function.ipynb          # Example of defining a simple function
│   ├── arguments_and_return.ipynb    # Function with arguments and return value
│   ├── default_parameters.ipynb      # Using default arguments
│   ├── positional_vs_keyword.ipynb   # Difference between positional and keyword arguments
├── mini_challenges
│   ├── square_function.ipynb         # Challenge: Write a function to calculate the square
│   ├── sum_list_function.ipynb       # Challenge: Write a function to sum a list
│   ├── calculator_function.ipynb     # Challenge: A calculator function with operations
├── project
│   ├── unit_converter.ipynb          # Project: Temperature unit converter
└── README.md                      
```


## **How to Use This Folder**

1. **Start with the Examples**:
   - Navigate to the `examples/` folder and review the basic concepts of functions.
   - Try running the scripts and experiment with the code.

2. **Practice with Mini Challenges**:
   - Go to the `mini_challenges/` folder.
   - Solve simple yet engaging coding exercises to reinforce your learning.

3. **Build a Mini Project**:
   - Check out the `project/` folder and run the **unit_converter.ipynb** script.
   - Modify the code to add your own features or conversions!



## **Highlights**

### **1. Basic Function**
Defining a simple function:
```python
def greet():
    print("Hello, World!")
```
Calling it:
```python
greet()  # Output: Hello, World!
```

### **2. Function with Arguments and Return Value**
Passing data into a function and receiving a result:
```python
def add_numbers(a, b):
    return a + b

result = add_numbers(5, 3)
print(result)  # Output: 8
```

### **3. Default Parameters**
Providing default values for parameters:
```python
def greet(name="User"):
    print(f"Hello, {name}!")

greet()         # Output: Hello, User!
greet("Alice")  # Output: Hello, Alice!
```

### **4. Positional vs Keyword Arguments**
Flexible argument passing:
```python
def describe_pet(name, species):
    print(f"{name} is a {species}.")

describe_pet("Buddy", "dog")            # Positional
describe_pet(species="cat", name="Milo")  # Keyword
```

---

## **Mini Challenges**
Test your skills with these exercises:
1. **Square Function**: Write a function that calculates the square of a number.
2. **Sum List Function**: Create a function to find the sum of a list.
3. **Calculator Function**: Build a simple calculator function that supports `+`, `-`, `*`, and `/`.

---

## **Project: Unit Converter**
Today’s project is a **Temperature Unit Converter**. Convert between Celsius and Fahrenheit using the function:
```python
def convert_temperature(value, unit="C"):
    if unit.upper() == "C":
        return (value * 9/5) + 32
    elif unit.upper() == "F":
        return (value - 32) * 5/9
    else:
        return "Invalid unit"

print(convert_temperature(100, "C"))  # Output: 212.0
print(convert_temperature(32, "F"))   # Output: 0.0
```

**Challenge**: Extend the project to include conversions for Kelvin or other units.


## **What’s Next?**
Tomorrow, you’ll learn about **Scope(global,local)** and **Lambda Functions**. Stay consistent and keep coding! 🚀

Happy Coding! 😊
