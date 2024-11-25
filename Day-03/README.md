# **Day 3: Basic I/O and String Manipulations**


## **What I Learned**
On Day 3, I focused on:
- **Basic Input/Output (I/O):** Taking input from users and displaying output using `input()` and `print()`.
- **String Manipulations:** Using Python's built-in methods and techniques to handle and modify strings.
- **String Indexing and Slicing:** Extracting specific parts of a string.
- **String Formatting:** Constructing formatted output using variables and expressions.


## **Key Concepts**

### **1. Input/Output Basics**
- Use `input()` to get input from the user (always returns a string).
- Use `print()` to display information.

**Example:**
```python
name = input("What is your name? ")
print(f"Hello, {name}!")
```


### **2. String Manipulation Methods**
| **Method**          | **Description**                               | **Example**                     |
|----------------------|-----------------------------------------------|----------------------------------|
| `lower()`            | Converts string to lowercase                 | `"Hello".lower()` -> `hello`    |
| `upper()`            | Converts string to uppercase                 | `"Hello".upper()` -> `HELLO`    |
| `strip()`            | Removes leading/trailing spaces              | `" Hello ".strip()` -> `Hello`  |
| `replace(old, new)`  | Replaces part of the string                  | `"hello".replace('h', 'H')` -> `Hello` |
| `split(separator)`   | Splits string into a list                    | `"a,b,c".split(',')` -> `['a', 'b', 'c']` |
| `join(iterable)`     | Joins elements of an iterable into a string  | `",".join(['a', 'b', 'c'])` -> `a,b,c` |
| `find(substring)`    | Finds the first occurrence of a substring    | `"hello".find('l')` -> `2`      |
| `len(string)`        | Returns the length of the string             | `len("hello")` -> `5`           |


### **3. String Indexing and Slicing**
- Strings are indexed from `0` for the first character.
- Negative indices access characters from the end (`-1` is the last character).
- Use slicing to extract parts of a string.

**Examples:**
```python
text = "Hello, Python!"

# Indexing
print(text[0])  # H
print(text[-1])  # !

# Slicing
print(text[0:5])  # Hello
print(text[7:])   # Python!
print(text[::-1])  # Reverse the string: !nohtyP ,olleH
```


### **4. String Formatting**
- Format strings using variables and expressions.

**Examples:**
1. **Using f-strings:**
   ```python
   name = "Alice"
   age = 25
   print(f"My name is {name} and I am {age} years old.")
   ```

2. **Using `.format()` method:**
   ```python
   print("My name is {} and I am {} years old.".format(name, age))
   ```

3. **String Concatenation:**
   ```python
   print("My name is " + name + " and I am " + str(age) + " years old.")
   ```


## **Code Examples**

### **Example 1: Basic I/O**
```python
name = input("Enter your name: ")
print(f"Hello, {name}!")
```


### **Example 2: String Methods**
```python
text = "  Hello, Python!  "

# Convert to lowercase and uppercase
print(text.lower())  # hello, python!
print(text.upper())  # HELLO, PYTHON!

# Remove spaces
print(text.strip())  # "Hello, Python!"

# Replace substring
print(text.replace("Python", "World"))  # "Hello, World!"
```


### **Example 3: String Slicing**
```python
text = "Hello, Python!"

# Indexing and Slicing
print(text[0])   # H
print(text[-1])  # !
print(text[0:5]) # Hello
print(text[::-1]) # Reverse string: !nohtyP ,olleH
```


## **Tasks**

### **Task 1: Reverse a String**
Write a program that reverses a user-provided string.

**Solution:**
```python
text = input("Enter a string: ")
reversed_text = text[::-1]
print(f"Reversed string: {reversed_text}")
```


### **Task 2: Count Vowels**
Write a program that counts the vowels in a given string.

**Solution:**
```python
text = input("Enter a string: ").lower()
vowels = "aeiou"
vowel_count = sum(1 for char in text if char in vowels)
print(f"Number of vowels: {vowel_count}")
```


### **Task 3: Format a Sentence**
Write a program to construct a formatted sentence based on user input.

**Solution:**
```python
name = input("What is your name? ")
hobby = input("What is your favorite hobby? ")
print(f"{name} loves {hobby}.")
```


## **What's Next?**
Next, I will explore **Day 4: Conditionals (`if`, `else`, `elif`)**.
