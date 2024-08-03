[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15499397&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

   * Python is a high-level, interpreted programming language known for its readability and simplicity. It was created by Guido van Rossum and first released in 1991. 
   * Python's key features include: - Easy to Read and Write: Python's syntax is clear and expressive, making it easy for beginners to learn and for developers to write code quickly.
   - Interpreted Language: Python code is executed line by line, which simplifies debugging and development.
   - Dynamically Typed: Variables in Python do not require explicit declaration, allowing for more flexible code.
   - Extensive Standard Library: Python comes with a vast standard library that supports many common programming tasks, such as file I/O, string manipulation, and data structures.
   - Large Community and Ecosystem: Python has a large community, which contributes to a rich ecosystem of libraries and frameworks, such as NumPy, Pandas, Django, and Flask.
   - Cross-Platform: Python runs on various platforms, including Windows, macOS, and Linux.
   * Use Cases: - Web Development: Using frameworks like Django and Flask.
   - Data Science and Machine Learning: Using libraries like Pandas, NumPy, SciPy, and scikit-learn.
   - Automation and Scripting: Automating repetitive tasks.
   Game Development: Using Libraries like Pygame.
   Embedded Systems: MicroPython and CircuitPython are used in embedded systems.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   * For Windows: 1. Download the Python installer from the official website (https://www.python.org/downloads/).
2. Run the installer and make sure to check the "Add Python to PATH" option.
3. Follow the installation prompts.
4. Verify the installation by opening Command Prompt and typing: python --version
* For macOS: 1. Open Terminal.
 2. Install Homebrew if not already installed: /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
3. Install Python using Homebrew: brew install python
4. Verify the installation: python3 --version
* For Linux: 1. Open Terminal.
2. Update the package list and install Python: sudo apt update
sudo apt install python3
3. Verify the installation: python3 --version
* Setting Up a Virtual Environment: 1. Install 'virtualenv' if not already installed: pip install virtualenv
2. Create a virtual envrironment: virtualenv myenv
3. Activate the virtual environment: Windows: myenv\Scripts\activate
  macOS: source myenv/bin/activate
4. Deactivate the virtual environment: deactivate


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   * print("Hello, World!) 
   - print: is a built-in function in Python that outputs text to the console.
   - The text to be printed is provided as an argument within parentheses and enclosed in double quotes.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   * Basic Data Types:

- Integer (int): Whole numbers, e.g., 42.
- Floating Point (float): Numbers with a decimal point, e.g., 3.14.
- String (str): Sequence of characters, e.g., "Hello".
- Boolean (bool): True or False values.
- List (list): Ordered collection of items, e.g., [1, 2, 3].
- Dictionary (dict): Collection of key-value pairs, e.g., {"name": "Alice", "age": 30}.
- Tuple (tuple): Ordered, immutable collection of items, e.g., (1, 2, 3).
- Set (set): Unordered collection of unique items, e.g., {1, 2, 3}.

* Script: 
# Integer
age = 25
print("Age:", age)

# Float
pi = 3.14159
print("PI:", pi)

# String
name = "John Doe"
print("Name:", name)

# Boolean
is_student = True
print("Is Student:", is_student)

# List
numbers = [1, 2, 3, 4, 5]
print("Numbers:", numbers)

# Dictionary
person = {"name": "Alice", "age": 30}
print("Person:", person)

# Tuple
coordinates = (10, 20)
print("Coordinates:", coordinates)

# Set
unique_numbers = {1, 2, 3, 4, 5}
print("Unique Numbers:", unique_numbers)


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an if-else statement and a for loop.

   * Conditional statements are used to execute code based on certain conditions. The basic structure is if, elif, and else.
   * Examples: 
   x = 10
if x > 0:
    print("x is positive")
elif x < 0:
    print("x is negative")
else:
    print("x is zero")

 * Loops: Loops are used to execute a block of code repeatedly. The basic loops in Python are for and while.
  * Example: 
  for i in range(5):
    print("Iteration:", i)


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   * Functions in Python are reusable blocks of code that perform a specific task. They are useful because they help in organizing code, reducing redundancy, and improving readability.
   * Example: def add_numbers(a, b):
    return a + b

# Calling the function
result = add_numbers(5, 3)
print("Sum:", result)

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   * Differences:

- List: Ordered collection of items, accessed by index.
- Dictionary: Collection of key-value pairs, accessed by keys.
 * Example: 
 # List of numbers
numbers = [10, 20, 30, 40, 50]
print("Numbers List:", numbers)

# Dictionary with key-value pairs
person = {"name": "Alice", "age": 30, "city": "New York"}
print("Person Dictionary:", person)

# Basic operations on list
numbers.append(60)
print("Updated Numbers List:", numbers)
print("Second Number:", numbers[1])

# Basic operations on dictionary
person["age"] = 31
print("Updated Person Dictionary:", person)
print("Person's Name:", person["name"])


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use try, except, and finally blocks to handle errors in a Python script.

   * Exception handling in Python allows you to handle runtime errors gracefully without crashing the program. It uses try, except, and finally blocks.
   * Example: 
   try:
    num1 = int(input("Enter a number: "))
    num2 = int(input("Enter another number: "))
    result = num1 / num2
    print("Result:", result)
except ZeroDivisionError:
    print("Error: Division by zero is not allowed.")
except ValueError:
    print("Error: Invalid input. Please enter a number.")
finally:
    print("Execution completed.")


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the math module.

   * Module: A file containing Python code, which can define functions, classes, and variables. It can be imported into other scripts.
   * Package: A collection of modules in directories that provide a hierarchical structure.
   * Example: 
   import math

# Using functions from the math module
print("Square root of 16:", math.sqrt(16))
print("Value of Pi:", math.pi)


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

    * Script: 
    # Reading from a file
try:
    with open('example.txt', 'r') as file:
        content = file.read()
        print("File Content:\n", content)
except FileNotFoundError:
    print("The file does not exist.")

# Writing to a file
lines = ["Hello, World!", "Python is great.", "File I/O is easy."]

with open('output.txt', 'w') as file:
    for line in lines:
        file.write(line + "\n")

print("Content written to output.txt")


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].