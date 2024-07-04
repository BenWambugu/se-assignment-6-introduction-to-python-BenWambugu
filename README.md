[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15370638&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
      Python is a high-level, interpreted programming language known for its simplicity and readability. Key features include dynamic typing, easy syntax, extensive standard libraries, and strong community support. It's popular for web development (Django, Flask), data analysis (Pandas, NumPy), automation (scripting), and AI/ML (TensorFlow, PyTorch).

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
      Installing Python on Windows:
Download Python Installer:

Go to the official Python website: python.org.
Navigate to the Downloads section and click on the latest Python release for Windows.
Run the Installer:

Once the download is complete, run the downloaded installer (python-3.x.x.exe).
Ensure to check the box that says "Add Python 3.x to PATH" during the installation process. This option allows you to run Python from the command line easily.
Customize Installation (Optional):

You can customize the installation by clicking on the "Customize installation" button. Here, you can select optional features and adjust the installation location if needed.
Complete the Installation:

Click "Install" to begin the installation process.
Once installation is complete, click on "Close" to exit the installer.
Verifying Python Installation:
To verify that Python is installed correctly on your Windows system:

Open Command Prompt:

Press Win + R, type cmd, and press Enter to open Command Prompt.
Check Python Version:

Type python --version or python -V and press Enter.
You should see the installed Python version (e.g., Python 3.9.6).
Check Python Interpreter:

Type python and press Enter to launch the Python interpreter.
You should see the Python prompt (>>>), indicating that Python is successfully installed and ready to use.
Setting Up a Virtual Environment:
Virtual environments allow you to manage and isolate dependencies for different projects. Here's how to set up a virtual environment using venv (a built-in Python module):

Create a Virtual Environment:

Open Command Prompt and navigate to your project directory using cd command.
Create a new virtual environment by running:
python -m venv myenv
Replace myenv with your preferred virtual environment name.
Activate the Virtual Environment:

To activate the virtual environment, run:
myenv\Scripts\activate
You should see (myenv) at the beginning of your Command Prompt prompt, indicating the virtual environment is active.
Verify Activation:

While the virtual environment is active, any Python commands (python, pip, etc.) will use the environment's Python interpreter and packages.


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   # Hello World program
      print("Hello, World!")

   The print() function is a built-in Python function that displays the specified message to the screen. The message "Hello, World!" is a string literal, which is a sequence of characters enclosed in double quotes (""). The function call is enclosed in parentheses (), which is the standard syntax for calling functions in Python. The entire line ends without a semicolon, as Python does not require semicolons to terminate statements, making the syntax clean and easy to read.



4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.


   Basic Data Types in Python
      Integer (int): Represents whole numbers, e.g., 10, -5.
      Floating-Point Number (float): Represents real numbers with decimal points, e.g., 3.14, -0.001.
      String (str): Represents sequences of characters, e.g., "Hello", 'Python'.
      Boolean (bool): Represents truth values, True or False.
      List (list): Ordered collection of items, e.g., [1, 2, 3], ["apple", "banana"].
      Tuple (tuple): Ordered, immutable collection of items, e.g., (1, 2, 3), ("apple", "banana").
      Dictionary (dict): Collection of key-value pairs, e.g., {"name": "Alice", "age": 30}.
      Set (set): Unordered collection of unique items, e.g., {1, 2, 3}, {"apple", "banana"}.

      # Integer
      age = 25
      print("Age:", age, type(age))

      # Float
      height = 5.9
      print("Height:", height, type(height))

      # String
      name = "Alice"
      print("Name:", name, type(name))

      # Boolean
      is_student = True
      print("Is Student:", is_student, type(is_student))

      # List
      fruits = ["apple", "banana", "cherry"]
      print("Fruits:", fruits, type(fruits))

      # Tuple
      coordinates = (10.0, 20.5)
      print("Coordinates:", coordinates, type(coordinates))

      # Dictionary
      person = {"name": "Bob", "age": 25}
      print("Person:", person, type(person))

      # Set
      unique_numbers = {1, 2, 3, 4, 4, 5}
      print("Unique Numbers:", unique_numbers, type(unique_numbers))


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   Conditional Statements (if-else): Used to make decisions in code. The if statement evaluates a condition and executes the corresponding block of code if the condition is True. The else statement provides an alternative block of code if the if condition is False.


   Loops (for): Used for iterating over sequences. The for loop in Python iterates over each item in a sequence (such as a list or string), assigning the item to a variable and executing a block of code for each item.

         # Example of if-else statement
      age = 18

      if age >= 18:
         print("You are an adult.")
      else:
         print("You are a minor.")

         # Example of a for loop
      fruits = ["apple", "banana", "cherry"]

      for fruit in fruits:
         print(fruit)

   


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

      Functions in Python are reusable blocks of code that perform a specific task. They allow for modular programming by encapsulating code into logical units, making the code more organized, readable, and easier to maintain. Functions can take inputs, perform operations, and return outputs.

            # Define the function
      def add_numbers(a, b):
         return a + b

      # Call the function
      result = add_numbers(5, 3)

      # Print the result
      print("The sum is:", result)


7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

      In Python, lists and dictionaries serve different purposes and have distinct characteristics. A list is an ordered collection of items, where each item is accessed by its index. Lists allow duplicate elements and support various operations such as append, remove, and sort. In contrast, a dictionary is an unordered collection of key-value pairs, where each key is unique and used to access its corresponding value. Dictionaries are optimized for fast lookups, insertions, and deletions using keys. While lists are typically used to store sequences of items, dictionaries are used to map unique keys to values, making them ideal for associative arrays or mappings.

            # Create a list of numbers
      numbers = [1, 2, 3, 4, 5]

      # Create a dictionary with key-value pairs
      person = {
         "name": "Alice",
         "age": 30,
         "city": "Nairobi"
      }

      # Basic operations on the list
      numbers.append(6)        # Add an element to the list
      numbers.remove(3)        # Remove an element from the list
      print("List of numbers:", numbers)
      print("Second element:", numbers[1])  # Access by index

      # Basic operations on the dictionary
      person["age"] = 31       # Update a value
      person["country"] = "Kenya"  # Add a new key-value pair
      print("Dictionary:", person)
      print("Name:", person["name"])  # Access by key



8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

   Exception handling in Python is a mechanism that allows you to manage and respond to runtime errors gracefully. Instead of letting the program crash, you can catch exceptions and handle them appropriately. This is done using try, except, and finally blocks. The try block contains code that might raise an exception, the except block catches and handles the exception, and the finally block contains code that will execute regardless of whether an exception occurred or not.

         # Example of exception handling

      def divide_numbers(a, b):
         try:
            # Code that might raise an exception
            result = a / b
            print("Result:", result)
         except ZeroDivisionError as e:
            # Code to handle the exception
            print("Error: Cannot divide by zero.")
            print("Exception message:", e)
         except TypeError as e:
            # Code to handle another type of exception
            print("Error: Invalid input type. Both arguments must be numbers.")
            print("Exception message:", e)
         finally:
            # Code that will always execute
            print("Execution completed.")

      # Test cases
      divide_numbers(10, 2)    # Valid division
      divide_numbers(10, 0)    # Division by zero
      divide_numbers(10, 'a')  # Invalid input type



9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

         Modules
      A module in Python is a single file (or files) that contains functions, classes, and variables which can be imported and used in other Python programs. Modules allow you to organize your code into separate files, making it easier to manage and reuse. A module can be a file containing Python code with a .py extension.

      Packages
      A package in Python is a collection of modules organized in directories that include a special file named __init__.py. The __init__.py file distinguishes a directory as a package, and it can be empty or contain initialization code for the package. Packages allow you to structure your project by grouping related modules together, making it easier to handle large codebases.

      Importing and Using a Module
      To use a module in your script, you need to import it using the import statement. You can import an entire module, specific functions, or use an alias.

      Example Using the math Module
      The math module provides access to various mathematical functions and constants. Here's an example of how to import and use the math module:

            # Import the entire math module
      import math

      # Use functions from the math module
      print("Square root of 16:", math.sqrt(16))
      print("Factorial of 5:", math.factorial(5))
      print("Value of pi:", math.pi)

      # Import specific functions from the math module
      from math import pow, ceil

      # Use the imported functions
      print("2 raised to the power 3:", pow(2, 3))
      print("Ceiling of 4.2:", ceil(4.2))

      # Import the math module with an alias
      import math as m

      # Use the alias to call functions
      print("Cosine of 0:", m.cos(0))



10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.


         Reading from and Writing to Files in Python
      Python provides built-in functions to handle file operations. The open() function is used to open a file, which returns a file object. You can then read from or write to this file object using various methods.

      Reading from a File
      To read from a file, you can use the open() function with the mode 'r' (read). You can read the entire content using the read() method or read line by line using a loop.

      Script to Read the Content of a File and Print It to the Console

            # Open the file in read mode
      with open('example.txt', 'r') as file:
         # Read the entire content of the file
         content = file.read()
         # Print the content to the console
         print(content)

            Writing to a File
      To write to a file, you can use the open() function with the mode 'w' (write) or 'a' (append). The write() method writes a string to the file, and the writelines() method writes a list of strings to the file.

      Script to Write a List of Strings to a File

            # List of strings to write to the file
      lines = [
         "Hello, World!\n",
         "Python is great.\n",
         "File handling is easy.\n"
      ]

      # Open the file in write mode
      with open('output.txt', 'w') as file:
         # Write the list of strings to the file
         file.writelines(lines)

      print("Data written to file successfully.")



# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


