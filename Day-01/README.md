### **Day 1: Introduction to Python, Installation, and IDEs**


#### **1. What is Python?**
- **Python** is a high-level, interpreted programming language known for its simplicity and readability.
- Created by **Guido van Rossum** and first released in 1991.
- It is widely used for web development, data science, automation, machine learning, and more.


#### **2. Why Learn Python?**
- **Beginner-Friendly:** Easy to read and write, making it ideal for beginners.
- **Versatile:** Used in various fields like web development, AI, data science, etc.
- **Large Community:** Extensive support from libraries and forums.
- **Cross-Platform:** Works on Windows, macOS, and Linux.


#### **3. Installing Python**
**Step-by-step guide to install Python:**

##### **Windows**
1. Go to the [official Python website](https://www.python.org/).
2. Download the latest version of Python.
3. Run the installer and make sure to check **"Add Python to PATH"** during installation.
4. Verify installation:
   - Open Command Prompt and type:
     ```
     python --version
     ```
   - It should return the installed version of Python.

##### **macOS**
1. Open Terminal and check if Python is pre-installed:
   ```
   python3 --version
   ```
   If not, install via [Homebrew](https://brew.sh/):
   ```
   brew install python
   ```

##### **Linux**
- Most Linux distributions come with Python pre-installed. To check:
  ```
  python3 --version
  ```
- To install or update:
  ```
  sudo apt update
  sudo apt install python3
  ```


#### **4. Setting Up an IDE**
An **Integrated Development Environment (IDE)** is a tool for writing, running, and debugging code. Below are popular options for Python:

1. **PyCharm (Recommended for Beginners)**
   - Download: [PyCharm Community Edition](https://www.jetbrains.com/pycharm/download/)
   - Install and configure Python interpreter.

2. **VS Code**
   - Install [VS Code](https://code.visualstudio.com/).
   - Add the **Python Extension** from the Extensions marketplace.

3. **Other IDEs:**
   - **Jupyter Notebook** (Best for data science and visualization).
   - **IDLE** (Comes pre-installed with Python).

---

#### **5. Writing Your First Python Program**
1. Open your IDE or a text editor (e.g., VS Code).
2. Create a new file called `hello.py`.
3. Write the following code:
   ```python
   print("Hello, Python!")
   ```
4. Save the file and run it:
   - In the terminal, navigate to the file directory and type:
     ```
     python hello.py
     ```
   - Output:
     ```
     Hello, Python!
     ```
