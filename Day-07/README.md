# **Day 7: Tuples and Sets**

Welcome to **Day 7** of the **100-Days-of-Python** series. Today, we dive into **tuples** and **sets**, which are foundational data structures in Python. You will learn how to use these collections effectively, understand their properties, and apply them in real-world scenarios.


## Topics Covered

### **1. Tuples**
- Immutable, ordered collections.
- Allow duplicate elements.
- Common use cases: storing fixed, unchangeable data, multiple return values, etc.

### **2. Sets**
- Unordered collections of unique elements.
- Useful for membership tests and performing mathematical set operations like union, intersection, and difference.


## Learning Objectives

By the end of this day, you will be able to:
1. Define and use tuples in Python.
2. Access and manipulate tuple elements.
3. Understand tuple immutability and how it affects operations.
4. Create and work with sets in Python.
5. Perform set operations (union, intersection, difference, symmetric difference).
6. Use set comprehensions for concise and efficient code.


## Folder Structure

```plaintext
Day7-Tuples-and-Sets
├── README.md               # Overview of Day 7
├── exercises               # Practice problems
│   ├── exercise1.py        # Sum of elements in a tuple
│   ├── exercise2.py        # Check if an element exists in a tuple
│   ├── exercise3.py        # Set operations
│   ├── exercise4.py        # Unique elements from a list using a set
│   ├── exercise5.py        # Adding duplicates to a set
├── examples                # Code examples for tuples and sets
│   ├── tuples_examples.py  # Examples covering tuple concepts
│   ├── sets_examples.py    # Examples covering set concepts
├── main.py                 # Summary script combining tuple and set operations
```


## Examples

### **Tuples**
#### Code Example:
```python
# Creating and accessing tuples
my_tuple = (10, 20, 30, 40)
print("Tuple:", my_tuple)
print("First Element:", my_tuple[0])
print("Slice:", my_tuple[1:3])
```

#### Output:
```plaintext
Tuple: (10, 20, 30, 40)
First Element: 10
Slice: (20, 30)
```


### **Sets**
#### Code Example:
```python
# Set operations
set1 = {1, 2, 3}
set2 = {3, 4, 5}

print("Union:", set1 | set2)
print("Intersection:", set1 & set2)
print("Difference:", set1 - set2)
print("Symmetric Difference:", set1 ^ set2)
```

#### Output:
```plaintext
Union: {1, 2, 3, 4, 5}
Intersection: {3}
Difference: {1, 2}
Symmetric Difference: {1, 2, 4, 5}
```


## Exercises

### **Exercise 1: Sum of Elements in a Tuple**
- **Objective**: Create a tuple of numbers and calculate their sum.
- **File**: `exercise1.py`

#### Example:
```python
numbers = (5, 10, 15, 20, 25)
print("Sum of elements:", sum(numbers))
```


### **Exercise 2: Check Element Existence in a Tuple**
- **Objective**: Check if a given element exists in a tuple.
- **File**: `exercise2.py`

#### Example:
```python
my_tuple = (10, 20, 30, 40, 50)
element = 30
if element in my_tuple:
    print(f"{element} exists in the tuple.")
```


### **Exercise 3: Set Operations**
- **Objective**: Perform union, intersection, and symmetric difference on two sets.
- **File**: `exercise3.py`

#### Example:
```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
print("Union:", set1 | set2)
```


## How to Use

1. Explore the **examples** folder to understand tuples and sets.
2. Solve the problems in the **exercises** folder to practice and solidify your understanding.
3. Run `main.py` to see a consolidated demonstration of tuple and set operations.


## Summary

Tuples and sets are powerful data structures in Python. Tuples provide a way to work with immutable sequences, while sets allow for efficient operations with unique elements. Mastering these concepts is essential for working with more advanced Python applications.


Happy coding! 🚀