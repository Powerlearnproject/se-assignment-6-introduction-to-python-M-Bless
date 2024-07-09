[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15390638&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
         -Python is a programming language that is widely used which is easily understood by most people.It is popular among developers because it is easy to interpret and friendly.
         -Some of the key features of python are:easy to learn and use,interpreted,dynamically typed and high level language.
         -Python is used in data science for instance while using the jupiter notebook.Frameworks of python are used in the development of python zuch as flask.
2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
         -print("Hello,World!")
          -Syntax elements used:-Function call...print() it outputs the specified message to the console.
                               -String.....the message printed
                               -Parentheses...enclose the argument in the function
4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
        -Integer:represent whole numbers without decimals.
        -Floating point numbers:represent real numbers with decimal point values.
        -String:represents statements and they are represented with double quotes.
        -Boolean:represent any of the two values True or False
        -List (list): An ordered, mutable collection of items, which can be of mixed types
        -Tuple (tuple): An ordered, immutable collection of items, which can be of mixed types
        -Dictionary (dict): An unordered collection of key-value pairs
        -Set (set): An unordered collection of unique items.

         # Integer
age = 30
print("Age:", age)
print("Type of age:", type(age))

# Float
height = 5.9
print("Height:", height)
print("Type of height:", type(height))

# String
name = "Alice"
print("Name:", name)
print("Type of name:", type(name))

# Boolean
is_student = True
print("Is student:", is_student)
print("Type of is_student:", type(is_student))

# List
fruits = ["apple", "banana", "cherry"]
print("Fruits:", fruits)
print("Type of fruits:", type(fruits))

# Tuple
coordinates = (10.0, 20.0)
print("Coordinates:", coordinates)
print("Type of coordinates:", type(coordinates))

# Dictionary
person = {"name": "Alice", "age": 30, "height": 5.9}
print("Person:", person)
print("Type of person:", type(person))

# Set
unique_numbers = {1, 2, 3, 4, 5}
print("Unique numbers:", unique_numbers)
print("Type of unique_numbers:", type(unique_numbers))

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
    -Conditional statements are statements that are used when a program is supposed to make more than one decision based on a certain condition.On the other hand,for loops are used to iterate a value until a certain condition is met.
          EXAMPLES: if(i==2):
                       print(2)
                    else:
                       print("Not two")
         EXAMPLES:for i in range(4)
6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
        -Functions are blocks of reusable code that are designed to perform a single related action.
        -Functions help in organizing and managing code by breaking down complex tasks into smaller, manageable pieces.
           EXAMPLE:
                def sum(a,b):
                  x=a+b
                 return x
               result=sum(2,4)
               print(result)

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
       -The difference between lists and dictionaries is that lists are an ordered, mutable collection of items, which can be of mixed types while dictionaries are  an unordered collection of key-value pairs.
          Example:
          # Creating a list of numbers
numbers = [1, 2, 3, 4, 5]
print("Original list:", numbers)

# Adding an element to the list
numbers.append(6)
print("List after appending 6:", numbers)

# Removing an element from the list
numbers.remove(3)
print("List after removing 3:", numbers)

# Accessing an element by index
print("Element at index 2:", numbers[2])

# Creating a dictionary with key-value pairs
person = {
    "name": "Alice",
    "age": 30,
    "city": "New York"
}
print("Original dictionary:", person)

# Adding a new key-value pair
person["occupation"] = "Engineer"
print("Dictionary after adding occupation:", person)

# Removing a key-value pair
del person["age"]
print("Dictionary after removing age:", person)

# Accessing a value by key
print("Person's name:", person["name"])

# Iterating through keys and values in the dictionary
for key, value in person.items():
    print(f"{key}: {value}")


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
       -Exception handling is a mechanism that allows you to mange errors gracefully and ensure the robustness of your programs.
          EXAMPLE:
            def divide(a, b):
    try:
        result = a / b
    except ZeroDivisionError as e:
        print("Error: Cannot divide by zero.")
        result = None
    else:
        print("Division successful.")
    finally:
        print("Execution completed.")
    return result

# Testing the function
print(divide(10, 2))  # Should print "Division successful." and return 5.0
print(divide(10, 0))  # Should print "Error: Cannot divide by zero." and return None

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
          -A module in Python is a single file (or files) that is intended to be imported and used in other Python programs. Modules allow you to organize your code into manageable sections and reuse code across multiple programs.
          -A package is a collection of related modules organized in a directory hierarchy. Packages allow you to structure your project into multiple sub-packages and modules, making it easier to manage and understand.
          EXAMPLE:
   import math

# Using math module functions
print("Square root of 16:", math.sqrt(16))  # Output: 4.0
print("Value of pi:", math.pi)              # Output: 3.141592653589793
print("Cosine of 0:", math.cos(0))          # Output: 1.0

# Using math module constants
radius = 5
area = math.pi * radius ** 2
print("Area of a circle with radius 5:", area)  # Output: 78.53981633974483

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

   -Open the File: Use the open() function to open a file in read mode ('r').
Read from the File: Use methods like read(), readline(), or readlines() to read data from the file.
Close the File: Always close the file using the close() method after reading is complete.

   EXAMPLE: 
        # Open the file in read mode
file_path = "sample.txt"
file = open(file_path, 'r')

# Read and print the entire content
content = file.read()
print("File Content:")
print(content)

# Close the file
file.close()
      
            WRITE:
    -Open the File: Use the open() function with write mode ('w') or append mode ('a') to open the file.
Write to the File: Use the write() method to write data to the file.
Close the File: Always close the file using the close() method after writing is complete to save the changes.
       EXAMPLE:
 # Open the file in write mode (creates a new file if it doesn't exist)
file_path = "output.txt"
file = open(file_path, 'w')

# Write to the file
file.write("This is line 1.\n")
file.write("This is line 2.\n")

# Close the file
file.close()

print(f"Successfully wrote to {file_path}")

   
# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


