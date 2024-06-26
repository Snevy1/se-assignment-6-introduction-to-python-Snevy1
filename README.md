[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15334220&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

      **Python**
      - Python is a dynamic, high-level, free open-source, and interpreted programming language.
      **Features**
      1. Easy to Learn and Read: Python’s straightforward syntax and indentation-based code blocks make it easy for beginners to learn and write code. Anyone can grasp Python basics in a few hours or days.
      2. Object-Oriented Language: Python supports object-oriented programming, including concepts like classes and object encapsulation.
      3. GUI Programming Support: You can create graphical user interfaces (GUIs) using modules like PyQt5, wxPython, or Tkinter. For instance, Instagram’s entire platform is built using Python and its Django framework
      4. Large Community Support: Python has a vast community on platforms like Stack Overflow, where questions are promptly answered.
      5. Portability: Python is portable across different platforms (Windows, Linux, Unix, Mac) without modification

      **Examples of use cases**
      - Web Applications: Python’s built-in frameworks (Django, Flask, Falcon) streamline web development
      - Software Development: Python is used to create various applications and platforms across industries
      - Data Science: Data scientists rely on Python for data analysis.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

      **Steps to install**
   1. Download the Installer:
     - Go to the official Python website: python.org.
     - Navigate to the Downloads section and click "Download Python 3.x.x" for Windows.
   2. Run the Installer:
     - Locate the downloaded file (usually in the Downloads folder) and run it.
     - Check the box that says "Add Python 3.x to PATH".
     - Click on "Install Now".
   3. Verify Installation:
     - Open Command Prompt (press Win + R, type cmd, and press Enter).
     - Type python --version or python -V and press Enter.
     - You should see the installed Python version.
   4. Set Up a Virtual Environment:
     - Open Command Prompt.
     - Navigate to your project directory.
     - Run python -m venv env (you can replace env with any name for your virtual environment).
     - To activate the virtual environment, run `.\env\Scripts\activate.`
     - You should see `(env)` in the command prompt, indicating the virtual environment is active.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   ```python
     print("Hello, world")

   ```
   - The print() is a function
   - The "Hello, world" string is the statement we want to print.


4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

    **Basic data types**
     1. Integers (int): Whole numbers without decimal points.
     2. Floating-Point Numbers (float): Numbers with decimal points.
     3. Complex Numbers (complex): Represented as a + bj, where a and b are real numbers
     4. Strings (str): Sequences of characters enclosed in single or double quotes.
     5. Lists (list): Ordered collections of items (can be of different types)
     6. Tuples (tuple): Similar to lists but immutable (cannot be modified after creation).
     7. Dictionaries (dict): Key-value pairs.
     8. Sets (set): Unordered collections of unique elements. 
     9. Booleans (bool): Represents True or False

     ```python
     # Creating variables
       age = 30
       price = 19.99
       name = "Alice"
       fruits = ["apple", "banana", "cherry"]
       coordinates = (10, 20)
       person = {"name": "John", "age": 36}
       is_sunny = True

    # Printing values
    print("Age:", age)
    print("Price:", price)
    print("Name:", name)
    print("Fruits:", fruits)
    print("Coordinates:", coordinates)
    print("Person:", person)
    print("Is it sunny?", is_sunny)
```
     
       

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   - Conditional statements in Python allow you to execute certain pieces of code based on whether a condition is true or false. The most common conditional statements are if, elif, and else.

   ```python
   age = 18

if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
```

- Loops allow you to execute a block of code multiple times. The most common types of loops in Python are for loops and while loops.

```python

   fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)
```




6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   - Functions are reusable blocks of code that perform specific tasks.

   ```python

   def add(a,b):
      return  a+b

     result =  add(4,6)

     print("Sum:", result)

     ```

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   - Lists are ordered collections of items while Dictionaries are unordered collections of key-value pairs.


   ```python

   # Creating a list of numbers
my_numbers = [10, 20, 30, 40]

# Creating a dictionary with key-value pairs
my_info = {'name': 'John', 'age': 25, 'country': 'USA'}

# Demonstrating basic operations:
print("List:")

print("Name:", my_info['name'])

```


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

   ** Exceptional handling**
   - Exception handling in Python is a way to manage errors that occur during the execution of a program. By using exception handling, you can write code that can respond to errors in a controlled way, instead of letting the program crash.
   - `try` block: This block contains the code that might throw an exception.
   - `except` block: This block contains the code that runs if an exception occurs in the `try` block.
   - `else` block: This block runs if no exception occurs in the `try` block (optional).
   - `finally` block: This block contains code that always runs, regardless of whether an exception occurred or not (optional).

   ```python

   try:
    # Code that might throw an exception
    numerator = 10
    denominator = 0
    result = numerator / denominator
    print("Result:", result)

except ZeroDivisionError as e:
    # Code to handle the exception
    print("Error: Division by zero is not allowed.")
    print("Exception message:", e)

else:
    # Code to execute if no exception occurs (optional)
    print("Division was successful.")

finally:
    # Code that always runs, regardless of exceptions (optional)
    print("Execution of the try-except block is complete.")
```


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

   1. Modules
     - A module is a single file containing Python code, such as functions, variables, and classes.
   2. Packages
     - A package is a collection of related modules organized in a directory hierarchy.
      **How to use**
     - To use a module, you import it using the import statement followed by the module’s name.
     - For example, to get the value of π (pi), you can use math.pi

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

    - Python provides built-in functions to read from and write to files. The most commonly used functions are open(), read(), readlines(), write(), and writelines().

    **Read from file**
    ```python
    # Script to read the content of a file and print it to the console
   file_path = 'example.txt'

 try:
    with open(file_path, 'r') as file:
        content = file.read()
        print(content)
  except FileNotFoundError:
    print(f"The file {file_path} does not exist.")
```

  **Write file**

  ```python

  # Script to write a list of strings to a file
  file_path = 'output.txt'
lines = [
    "Line 1: This is the first line.\n",
    "Line 2: This is the second line.\n",
    "Line 3: This is the third line.\n"
]

try:
    with open(file_path, 'w') as file:
        file.writelines(lines)
    print(f"Content written to {file_path} successfully.")
except Exception as e:
    print(f"An error occurred: {e}")

    ```


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


