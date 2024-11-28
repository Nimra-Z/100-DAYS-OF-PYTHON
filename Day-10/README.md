# **Day 10: Scope and Lambda Functions**

Welcome to **Day 10** of the **100 Days of Python Challenge**! 🎉  
Today, we’ll explore two powerful and essential concepts in Python:

1. **Scope**: How and where variables are accessible in your code.
2. **Lambda Functions**: Writing concise, one-liner anonymous functions for quick tasks.

By the end of the day, you’ll understand variable scope, master the `lambda` keyword, and use these tools to write cleaner and more efficient code.


## **Topics Covered**

### 1. **Scope**  
Scope determines the visibility of variables in your program:
- **Local Scope**: Variables defined inside a function.
- **Global Scope**: Variables defined outside any function and accessible globally.
- **The `global` Keyword**: Modify global variables from within a function.

### 2. **Lambda Functions**  
A lambda function is a small, anonymous function:
- Written as `lambda arguments: expression`.
- Used for short, simple operations.
- Commonly applied with functions like `map()`, `filter()`, and `sorted()`.


## **Folder Structure**

```
Day_10_Scope_and_Lambda
├── examples
│   ├── scope_global_vs_local.ipynb         # Examples of local vs global variables
│   ├── global_keyword.ipynb                # Using the `global` keyword
│   ├── lambda_basics.ipynb                 # Basic lambda functions
│   ├── lambda_with_map_filter_sorted.ipynb # Lambda with map, filter, and sorted
├── mini_challenges
│   ├── calculate_area.ipynb                # Lambda for rectangle area calculation
│   ├── sort_names.ipynb                    # Lambda to sort names by length
│   ├── square_odd_numbers.ipynb            # Lambda to filter and square odd numbers
├── project
│   ├── lambda_calculator.ipynb             # A calculator using lambda functions
└── README.md                         
```



## **How to Use This Folder**

1. **Start with the Examples**:  
   - Navigate to the `examples/` folder.
   - Run the Python scripts to understand the basics of scope and lambda functions.

2. **Practice with Mini Challenges**:  
   - Go to the `mini_challenges/` folder.
   - Solve coding exercises to strengthen your understanding.

3. **Explore the Project**:  
   - Check out the `project/` folder to see a real-world use case of lambda functions.
   - Extend the functionality of the calculator project to add more operations!



## **Highlights**

### **1. Scope: Local vs Global**

```python
# Local variable example
def greet():
    message = "Hello, Local Scope!"  # Local variable
    print(message)

greet()
# print(message)  # Error: message is not accessible outside the function

# Global variable example
name = "Alice"  # Global variable

def greet_global():
    print(f"Hello, {name}!")  # Accessing global variable

greet_global()  # Output: Hello, Alice!
```

### **2. Using the `global` Keyword**

```python
# Global variable example
counter = 0

def increment():
    global counter  # Access global variable
    counter += 1

increment()
print(counter)  # Output: 1
```

### **3. Lambda Functions**

```python
# Lambda function to calculate square
square = lambda x: x ** 2
print(square(4))  # Output: 16

# Lambda function for addition
add = lambda a, b: a + b
print(add(3, 5))  # Output: 8
```

### **4. Using Lambda with `map()`, `filter()`, and `sorted()`**

```python
numbers = [1, 2, 3, 4, 5]

# Squaring numbers using map
squared = list(map(lambda x: x ** 2, numbers))
print(squared)  # Output: [1, 4, 9, 16, 25]

# Filtering odd numbers
odds = list(filter(lambda x: x % 2 != 0, numbers))
print(odds)  # Output: [1, 3, 5]

# Sorting numbers in descending order
sorted_desc = sorted(numbers, key=lambda x: -x)
print(sorted_desc)  # Output: [5, 4, 3, 2, 1]
```


## **Mini Challenges**

### Challenge 1: **Calculate Area**
Write a lambda function to calculate the area of a rectangle:
```python
area = lambda length, width: length * width
print(area(5, 10))  # Output: 50
```


### Challenge 2: **Sort Names**
Use a lambda function to sort a list of names by their length:
```python
names = ["Alice", "Bob", "Charlie", "Diana"]
sorted_names = sorted(names, key=lambda name: len(name))
print(sorted_names)  # Output: ['Bob', 'Alice', 'Diana', 'Charlie']
```


### Challenge 3: **Square Odd Numbers**
Filter a list to include only odd numbers, then square them:
```python
numbers = [1, 2, 3, 4, 5]
squared_odds = list(map(lambda x: x ** 2, filter(lambda x: x % 2 != 0, numbers)))
print(squared_odds)  # Output: [1, 9, 25]
```


## **Project: Lambda Calculator**

Build a simple calculator using lambda functions:
```python
# Lambda functions for basic operations
add = lambda a, b: a + b
subtract = lambda a, b: a - b
multiply = lambda a, b: a * b
divide = lambda a, b: a / b if b != 0 else "Error: Division by zero"

# Using the calculator
print(add(10, 5))         # Output: 15
print(subtract(10, 5))    # Output: 5
print(multiply(10, 5))    # Output: 50
print(divide(10, 5))      # Output: 2.0
print(divide(10, 0))      # Output: Error: Division by zero
```

**Challenge**: Extend the calculator to include operations like modulus (`%`), exponentiation (`**`), and square root.


## **What’s Next?**

Tomorrow, we’ll dive into **Modules** — learning how to import, use, and even create your own modules to supercharge your Python projects.

Keep up the great work, and happy coding! 🚀
