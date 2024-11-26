# **Day 8: Dictionaries and Dictionary Methods**

Welcome to **Day 8** of the 100-Days-of-Python series! Today, we explore one of Python's most powerful and versatile data structures: **Dictionaries**. They allow you to store and manipulate data as key-value pairs efficiently.


## What You’ll Learn

### Key Concepts:
- Understanding dictionaries and their use cases.
- Creating dictionaries.
- Accessing, adding, updating, and deleting key-value pairs.
- Using dictionary methods like `.keys()`, `.values()`, `.items()`, and `.get()`.
- Iterating through dictionaries.

### Practical Applications:
- Analyzing data frequency using dictionaries.
- Building dynamic and user-friendly applications like contact books and inventory systems.
- Saving and retrieving dictionaries to/from files.


## Folder Structure

```
Day08-Dictionaries
│
├── README.md
├── examples
│   ├── basics.py             # Demonstrates basic dictionary operations.
│   ├── methods.py            # Shows usage of key dictionary methods.
│   └── iteration.py          # Examples of iterating through dictionaries.
├── exercises
│   ├── exercise1.py          # Practice creating and modifying dictionaries.
│   ├── exercise2.py          # Character frequency counter using a dictionary.
│   └── frequency_counter.py  # Word and character frequency analysis.
├── tasks
│   ├── dictionary_manager.py # A CLI-based dictionary manager.
│   └── mini_projects.md      # Ideas for extending learning into real-world applications.
└── projects
    ├── frequency_analyzer.py # Analyzes word and character frequency in a string.
    ├── contact_book.py       # Personal contact book with add, update, and delete features.
    ├── inventory_system.py   # A simple inventory management system.
    └── json_storage.py       # Saving and loading dictionaries like JSON.
```


## Examples

### Basic Dictionary Operations (`examples/basics.py`)
```python
# Create a dictionary
person = {"name": "Alice", "age": 25, "city": "New York"}

# Access a value
print(person["name"])  # Output: Alice

# Add or update a key-value pair
person["gender"] = "Female"
print(person)

# Delete a key
del person["city"]
print(person)
```

### Key Methods (`examples/methods.py`)
```python
person = {"name": "Alice", "age": 25}

# Get all keys
print(person.keys())  # Output: dict_keys(['name', 'age'])

# Get all values
print(person.values())  # Output: dict_values(['Alice', 25])

# Iterate over key-value pairs
for key, value in person.items():
    print(f"{key}: {value}")
```


## Mini Projects

### 1. Frequency Analyzer (`projects/frequency_analyzer.py`)
- **Input**: A long string.
- **Output**: Frequency of each word and each character.
- **Usage**: Useful for analyzing text data.

### 2. Personal Contact Book (`projects/contact_book.py`)
- A dynamic program to store, update, delete, and search for contacts.
- Includes user-friendly CLI navigation.

### 3. Simple Inventory System (`projects/inventory_system.py`)
- Manage a shop’s inventory by tracking item prices and quantities.
- Features addition, update, deletion, and review of inventory.

### 4. JSON-like Dictionary Storage (`projects/json_storage.py`)
- Save dictionaries to a file and load them back for persistent storage.
- Works like a lightweight database for small projects.


## Exercises

### Exercise 1: Create and Modify a Dictionary (`exercises/exercise1.py`)
- Create a dictionary with personal details.
- Add a new key, update an existing one, and delete a key.

### Exercise 2: Character Frequency Counter (`exercises/exercise2.py`)
- Write a program to count the frequency of each character in a string.
- Use `.get()` to simplify dictionary updates.


## Tasks

### Build a Dictionary Manager (`tasks/dictionary_manager.py`)
A CLI-based application where users can:
- Add, update, delete, and view key-value pairs dynamically.
- Exit the program after saving changes.


Happy coding! 🚀