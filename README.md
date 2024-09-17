# Python Tutorial: From Scratch to Professional

Welcome to **Python Tutorial: From Scratch to Professional!** Whether you're completely new to programming or aiming to take your Python skills to a professional level, this tutorial has got you covered. With detailed explanations, practical examples, and step-by-step guidance, you’ll be able to confidently write Python code and build real-world applications.

---

## Table of Contents

1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Getting Started](#getting-started)
    - [1. Installing Python](#1-installing-python)
    - [2. Writing Your First Program](#2-writing-your-first-program)
4. [Basic Concepts](#basic-concepts)
    - [3. Variables and Data Types](#3-variables-and-data-types)
    - [4. Conditional Statements](#4-conditional-statements)
    - [5. Loops](#5-loops)
    - [6. Functions](#6-functions)
5. [Intermediate Concepts](#intermediate-concepts)
    - [7. File Handling](#7-file-handling)
    - [8. Object-Oriented Programming](#8-object-oriented-programming)
    - [9. Modules and Packages](#9-modules-and-packages)
6. [Advanced Concepts](#advanced-concepts)
    - [10. Exception Handling](#10-exception-handling)
    - [11. Working with APIs](#11-working-with-apis)
    - [12. Advanced Data Structures](#12-advanced-data-structures)
7. [Projects](#projects)
    - [13. Building a Web Scraper](#13-building-a-web-scraper)
    - [14. Developing a REST API](#14-developing-a-rest-api)
    - [15. Machine Learning with Python](#15-machine-learning-with-python)
8. [Resources](#resources)

---

## Introduction

This tutorial is for absolute beginners and those looking to enhance their Python skills. You will learn everything from how to install Python, write basic programs, and tackle real-world projects like creating APIs or machine learning models.

## Prerequisites

- Basic understanding of how to use a computer
- A text editor (e.g., VS Code, PyCharm, Sublime Text)
- Python installed on your system (instructions below)

---

## Getting Started

### 1. Installing Python

To start using Python, you need to install it on your computer. Follow these steps:

#### Windows:

1. Go to [Python's official website](https://www.python.org/downloads/) and download the latest version.
2. During installation, make sure to check the box "Add Python to PATH".
3. Open Command Prompt and verify the installation:

```bash
python --version
```

#### macOS/Linux:

1. Open a terminal and run:

```bash
brew install python  # On macOS using Homebrew
```

2. For Linux, use your package manager:

```bash
sudo apt-get install python3
```

### 2. Writing Your First Program

After installing Python, let's write a simple "Hello, World!" program.

```python
# hello.py
print("Hello, World!")
```

#### Explanation:

- `print()` is a built-in function that outputs text to the console.
- `"Hello, World!"` is a string, which is a sequence of characters.

Save this file as `hello.py` and run it in the terminal:

```bash
python hello.py
```

You should see: `Hello, World!`

---

## Basic Concepts

### 3. Variables and Data Types

In Python, variables store data. The type of data a variable holds can be an integer, a string, a float, or a boolean. Python automatically determines the type of variable based on the value you assign to it.

```python
# Example of different data types in Python
name = "Alice"        # String
age = 25              # Integer
height = 5.7          # Float
is_student = True     # Boolean
```

#### Explanation:

- **String**: A sequence of characters (e.g., `"Alice"`).
- **Integer**: A whole number without a decimal point (e.g., `25`).
- **Float**: A number with a decimal point (e.g., `5.7`).
- **Boolean**: A value that can be either `True` or `False`.

```python
# Example: Using variables in a print statement
print(f"Name: {name}, Age: {age}, Height: {height}, Student: {is_student}")
```

Output:

```
Name: Alice, Age: 25, Height: 5.7, Student: True
```

### 4. Conditional Statements

Conditional statements allow you to execute different blocks of code depending on whether a condition is `True` or `False`.

```python
# Example: Checking if a person is an adult
age = 20
if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
```

#### Explanation:

- `if age >= 18:` checks if the age is greater than or equal to 18.
- The code under `if` runs when the condition is `True`; otherwise, the code under `else` runs.

### 5. Loops

Python has two main types of loops: **for loops** and **while loops**. Loops help you repeat code.

#### For Loop:

```python
# Example: Print numbers from 0 to 4
for i in range(5):
    print(f"Iteration {i}")
```

#### Explanation:

- `range(5)` generates numbers from 0 to 4.
- `for i in range(5):` repeats the loop for each number in that range, assigning each value to `i`.

#### While Loop:

```python
# Example: Count to 5 using a while loop
count = 0
while count < 5:
    print(f"Count: {count}")
    count += 1  # Increment count by 1
```

#### Explanation:

- `while count < 5:` keeps running as long as the condition is `True`.
- `count += 1` increases the value of `count` by 1 after each iteration.

### 6. Functions

A **function** is a reusable block of code that performs a specific task.

```python
# Example: Define and call a function
def greet(name):
    """This function greets the person whose name is passed as an argument."""
    return f"Hello, {name}!"

print(greet("Alice"))
```

#### Explanation:

- `def greet(name):` defines a function called `greet` that accepts a parameter `name`.
- `return` sends the result of the function back to where it was called.
- `"""` is a **docstring** that provides documentation for the function.

### 7. Lists, Tuples, and Dictionaries

Python provides several data structures to store collections of items.

#### Lists:

A list is a collection of ordered, changeable, and indexed items.

```python
# Example: Creating a list of fruits
fruits = ["apple", "banana", "cherry"]
print(fruits[1])  # Output: banana
```

#### Explanation:

- Lists are created using square brackets `[ ]`.
- Items in a list are indexed starting from 0.

#### Tuples:

A tuple is a collection of ordered and unchangeable items.

```python
# Example: Creating a tuple
person = ("Alice", 25, "Engineer")
print(person[0])  # Output: Alice
```

#### Explanation:

- Tuples are created using parentheses `( )`.
- Unlike lists, you cannot change the values in a tuple after it’s created.

#### Dictionaries:

A dictionary is a collection of unordered, changeable, and indexed items. It stores data as key-value pairs.

```python
# Example: Creating a dictionary
student = {"name": "Alice", "age": 25, "course": "Math"}
print(student["name"])  # Output: Alice
```

#### Explanation:

- Dictionaries use curly braces `{ }`.
- Keys in a dictionary must be unique.

---

## Intermediate Concepts

### 8. File Handling

In Python, you can easily work with files.

```python
# Writing to a file
with open('sample.txt', 'w') as file:
    file.write("This is a sample file.")
```

```python
# Reading from a file
with open('sample.txt', 'r') as file:
    content = file.read()
    print(content)
```

#### Explanation:

- `open()` is used to open a file in different modes (`'w'` for writing, `'r'` for reading).
- `with` ensures that the file is properly closed after the block of code runs.

### 9. Object-Oriented Programming

Object-Oriented Programming (OOP) allows you to define classes and create objects from those classes.

```python
# Example: Defining a class and creating an object
class Dog:
    def __init__(self, name, breed):
        self.name = name
        self.breed = breed

    def bark(self):
        return f"{self.name} is

 barking."

# Creating an object of class Dog
my_dog = Dog("Buddy", "Golden Retriever")
print(my_dog.bark())  # Output: Buddy is barking.
```

#### Explanation:

- `class Dog:` defines a class called `Dog`.
- `__init__()` is the constructor method that initializes the object.
- `my_dog = Dog("Buddy", "Golden Retriever")` creates an object `my_dog` with the specified attributes.

---

## Assignment: Fix the Code Quizzes

As part of this Python tutorial, you will be presented with several coding quizzes. Your task is to fix the errors in the provided code or complete the logic where necessary. Each quiz will challenge different aspects of Python, from basic syntax to advanced concepts like object-oriented programming and file handling.

### How to Use:

1. Copy the code.
2. Read the code and the hint provided.
3. Fix the code or complete the logic as instructed.
4. Test the code to ensure it runs correctly.

---

### Quiz 1: Fix the Variable Assignment

**Problem:** The program should print the value of `age` but currently throws an error.

```python
# quiz_1.py

# Hint: There is a mistake in how the variable is assigned.
age = "25 years"
print(Age)
```

---

### Quiz 2: Debug the If-Else Statement

**Problem:** The code is supposed to check if a person is eligible to vote, but it has a logical error.

```python
# quiz_2.py

# Hint: Check the condition inside the if statement.
age = 16
if age > 18:
    print("Eligible to vote")
else:
    print("Not eligible to vote")
```

---

### Quiz 3: Complete the Loop

**Problem:** The loop is incomplete, and it should print all even numbers from 1 to 10.

```python
# quiz_3.py

# Hint: You need to modify the loop condition to meet the criteria.
for i in range(1, 10):
    if i % 2 == 0:
        print(i)
```

---

### Quiz 4: Fix the Function Return

**Problem:** This function should return the square of a number, but it currently does nothing.

```python
# quiz_4.py

# Hint: Make sure the function returns a value.
def square(num):
    num * num

print(square(4))
```

---

### Quiz 5: Correct the String Formatting

**Problem:** The code should print a greeting message using the `name` variable, but there’s a mistake in the formatting.

```python
# quiz_5.py

# Hint: Use the correct method to format strings in Python.
name = "Alice"
print("Hello, {}!")
```

---

### Quiz 6: Debug the List Access

**Problem:** The program tries to access an element in the list but throws an IndexError.

```python
# quiz_6.py

# Hint: Check the list indexing.
fruits = ["apple", "banana", "cherry"]
print(fruits[3])
```

---

### Quiz 7: Fix the File Handling

**Problem:** The program should read and print the content of `data.txt`, but it currently raises an error.

```python
# quiz_7.py

# Hint: Ensure that the file is opened in the correct mode and check the file path.
with open('data.txt', 'w') as f:
    print(f.read())
```

---

### Quiz 8: Correct the Class Definition

**Problem:** The class `Car` should have a method to display its attributes, but the code currently throws an error.

```python
# quiz_8.py

# Hint: Make sure to properly define the class and its methods.
class Car:
    def __init__(self, make, model):
        make = make
        model = model

    def display(self):
        print("Make: " + make + ", Model: " + model)

car = Car("Toyota", "Corolla")
car.display()
```

---

### Quiz 9: Fix the Dictionary Lookup

**Problem:** The program should return the capital of France from the dictionary, but it fails.

```python
# quiz_9.py

# Hint: Ensure the correct key is used when accessing dictionary values.
capitals = {"USA": "Washington, D.C.", "France": "Paris", "Japan": "Tokyo"}
print(capitals["france"])
```

---

### Quiz 10: Correct the List Sorting

**Problem:** The program tries to sort a list of numbers but throws a TypeError.

```python
# quiz_10.py

# Hint: Look carefully at the data types in the list.
numbers = [1, 2, 'three', 4, 5]
print(sorted(numbers))
```

---

### Quiz 11: Fix the Import Statement

**Problem:** The code is supposed to calculate the area of a circle using `math.pi`, but it throws a NameError.

```python
# quiz_11.py

# Hint: Make sure to import the necessary module for using `pi`.
radius = 5
area = pi * radius ** 2
print(area)
```

---

### Quiz 12: Complete the Decorator

**Problem:** The decorator is supposed to print a message before and after calling the function, but it’s incomplete.

```python
# quiz_12.py

# Hint: Add the missing logic to the decorator function.
def my_decorator(func):
    def wrapper():
        print("Before function call")
        func()
        print("After function call")
    return wrapper

@my_decorator
def say_hello():
    print("Hello!")

say_hello()
```

---

This concludes the coding quizzes section. Fixing these problems will help you strengthen your Python debugging and problem-solving skills. Each quiz is designed to focus on common mistakes and best practices that will help you in real-world coding challenges.

---

This README continues into **Advanced Concepts**, **Projects**, and additional **Resources**. 
