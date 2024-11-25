# **Day 6: Lists and List Methods**


## **What I Learned**
On Day 6, I explored:
- Using **lists** to store and manage collections of data.
- Common **list methods** for adding, removing, and organizing elements.
- Iterating through lists using loops for dynamic processing.


## **Key Concepts**

### **1. What is a List?**
- A **list** is an ordered, mutable collection of items.
- Items in a list can be of different data types.

**Example:**
```python
fruits = ["apple", "banana", "cherry"]
print(fruits[0])  # Output: apple
```


### **2. Common List Operations**
- **Access Elements:** Use indexing (`list[index]`).
- **Modify Elements:** Assign a value to a specific index.
- **Add Elements:** Use `append()`, `extend()`, or `insert()`.
- **Remove Elements:** Use `remove()`, `pop()`, or `del`.
- **Iterate:** Use loops to traverse through a list.


### **3. Common List Methods**
| **Method**          | **Description**                                      | **Example**                   |
|----------------------|------------------------------------------------------|--------------------------------|
| `append(item)`       | Adds an item to the end of the list                  | `fruits.append("grape")`      |
| `remove(item)`       | Removes the first occurrence of the specified item   | `fruits.remove("apple")`      |
| `sort()`             | Sorts the list in ascending order                    | `numbers.sort()`              |
| `reverse()`          | Reverses the order of the list                       | `numbers.reverse()`           |
| `count(item)`        | Counts occurrences of an item in the list            | `numbers.count(2)`            |


### **4. Iterating Through a List**
**Example:**
```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)  # Prints each fruit in the list
```


## **Code Examples**

### **1. Basic List Operations**
```python
# Create and access a list
numbers = [10, 20, 30, 40, 50]
print(numbers[0])  # Output: 10
numbers[2] = 35  # Modify an element
print(numbers)  # Output: [10, 20, 35, 40, 50]
```


### **2. Adding and Removing Elements**
```python
# Add elements
fruits = ["apple", "banana"]
fruits.append("cherry")
print(fruits)  # Output: ['apple', 'banana', 'cherry']

# Remove elements
fruits.remove("banana")
print(fruits)  # Output: ['apple', 'cherry']
```


### **3. Sorting and Reversing a List**
```python
numbers = [5, 2, 9, 1, 7]
numbers.sort()  # Sort in ascending order
print(numbers)  # Output: [1, 2, 5, 7, 9]

numbers.reverse()  # Reverse the list
print(numbers)  # Output: [9, 7, 5, 2, 1]
```


### **4. Iterating Through a List**
```python
names = ["Alice", "Bob", "Charlie"]
for name in names:
    print(f"Hello, {name}!")
```


## **Tasks**

### **Task 1: Find the Largest Number**
Write a program to find the largest number in a list.

**Solution:**
```python
numbers = [10, 50, 20, 80, 60]
largest = max(numbers)
print(f"The largest number is {largest}.")
```


### **Task 2: Count Occurrences**
Write a program to count how many times a specific element appears in a list.

**Solution:**
```python
numbers = [1, 2, 2, 3, 4, 2, 5]
target = 2
count = numbers.count(target)
print(f"{target} appears {count} times in the list.")
```


### **Task 3: Create a Shopping List**
Write a program that:
1. Allows the user to add items to a shopping list.
2. Lets the user remove items from the list.
3. Displays the list when the user is done.

**Solution:**
```python
shopping_list = []

while True:
    action = input("Enter 'add', 'remove', or 'done': ").lower()
    if action == "add":
        item = input("Enter an item to add: ")
        shopping_list.append(item)
    elif action == "remove":
        item = input("Enter an item to remove: ")
        if item in shopping_list:
            shopping_list.remove(item)
        else:
            print(f"{item} is not in the shopping list.")
    elif action == "done":
        break
    else:
        print("Invalid action.")

print("Your shopping list:")
print(shopping_list)
```


## **What's Next?**
Next, I will explore **Day 7: Tuples and Sets**.
