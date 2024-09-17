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

## Projects: Hands-On Practice

To further solidify your Python knowledge, here are some hands-on projects that you can work on. These projects are designed to challenge your understanding of key concepts and give you practical experience.

### Project 1: Simple To-Do List (Beginner)

**Objective:** Create a command-line to-do list application where users can add, remove, and view tasks.

**Concepts Covered:**
- Functions
- Lists
- Loops
- User input

**Example:**

```python
tasks = []

def add_task(task):
    tasks.append(task)
    print(f"'{task}' added to the list.")

def remove_task(task):
    tasks.remove(task)
    print(f"'{task}' removed from the list.")

def show_tasks():
    print("Your to-do list:")
    for task in tasks:
        print(f"- {task}")

# Example usage
add_task("Learn Python")
show_tasks()
remove_task("Learn Python")
```

### Project 2: Dice Rolling Simulator (Intermediate)

**Objective:** Create a program that simulates rolling dice. The user should be able to input the number of sides on the dice and the number of rolls.

**Concepts Covered:**
- Random number generation
- Functions
- Loops

**Example:**

```python
import random

def roll_dice(sides, rolls):
    for i in range(rolls):
        print(f"Roll {i+1}: {random.randint(1, sides)}")

# Example usage
sides = 6
rolls = 3
roll_dice(sides, rolls)
```

### Project 3: Budget Tracker (Intermediate)

**Objective:** Build a simple budget tracker where users can add income and expenses and see their current balance.

**Concepts Covered:**
- Dictionaries
- Functions
- Loops

**Example:**

```python
budget = {"income": 0, "expenses": 0}

def add_income(amount):
    budget["income"] += amount
    print(f"Added income: {amount}")

def add_expense(amount):
    budget["expenses"] += amount
    print(f"Added expense: {amount}")

def show_balance():
    balance = budget["income"] - budget["expenses"]
    print(f"Current balance: {balance}")

# Example usage
add_income(1000)
add_expense(500)
show_balance()
```

### Project 4: Rock, Paper, Scissors Game (Intermediate)

**Objective:** Create a Rock, Paper, Scissors game where the user plays against the computer. The program should randomly select the computer's choice and determine the winner.

**Concepts Covered:**
- Random choice
- Functions
- Conditionals

**Example:**

```python
import random

def play_game():
    user_choice = input("Enter rock, paper, or scissors: ").lower()
    options = ["rock", "paper", "scissors"]
    computer_choice = random.choice(options)

    print(f"Computer chose: {computer_choice}")

    if user_choice == computer_choice:
        print("It's a tie!")
    elif (user_choice == "rock" and computer_choice == "scissors") or \
         (user_choice == "scissors" and computer_choice == "paper") or \
         (user_choice == "paper" and computer_choice == "rock"):
        print("You win!")
    else:
        print("You lose!")

# Example usage
play_game()
```

### Project 5: Contact Book (Advanced)

**Objective:** Build a contact book where users can store, view, edit, and delete contact information (name, phone number, and email). The data should be stored in a file.

**Concepts Covered:**
- File handling
- Dictionaries
- Functions
- User input

**Example:**

```python
contacts = {}

def add_contact(name, phone, email):
    contacts[name] = {"phone": phone, "email": email}
    print(f"Contact {name} added.")

def remove_contact(name):
    if name in contacts:
        del contacts[name]
        print(f"Contact {name} removed.")
    else:
        print("Contact not found.")

def show_contacts():
    for name, info in contacts.items():
        print(f"{name}: Phone - {info['phone']}, Email - {info['email']}")

# Example usage
add_contact("Alice", "1234567890", "alice@example.com")
show_contacts()
remove_contact("Alice")
```

### Project 6: Weather App (Advanced)

**Objective:** Build a weather app that fetches real-time weather data from an API (e.g., OpenWeatherMap) and displays it to the user based on their city input.

**Concepts Covered:**
- APIs (using requests)
- JSON parsing
- Functions
- User input

**Example:**

```python
import requests

def get_weather(city):
    api_key = 'your_api_key_here'
    base_url = f"http://api.openweathermap.org/data/2.5/weather?q={city}&appid={api_key}"
    response = requests.get(base_url)
    data = response.json()

    if data['cod'] == 200:
        temp = data['main']['temp'] - 273.15  # Convert from Kelvin to Celsius
        weather = data['weather'][0]['description']
        print(f"The temperature in {city} is {temp:.2f}°C with {weather}.")
    else:
        print("City not found.")

# Example usage
city = input("Enter your city: ")
get_weather(city)
```

---

## Additional Resources

Here are some valuable resources to help you dive deeper into Python programming and enhance your skills beyond this tutorial.

### Official Documentation

- [Python Documentation](https://docs.python.org/3/): The official documentation is a great place to look for in-depth explanations of Python features and functions.

### Free Learning Platforms

- [Codecademy](https://www.codecademy.com/learn/learn-python-3): Offers an interactive Python course suitable for beginners.
- [Kaggle](https://www.kaggle.com/learn/python): Great for hands-on learning with datasets and machine learning.

### Books

- **“Python Crash Course”** by Eric Matthes: A great book for beginners that also includes advanced projects.
- **“Automate the Boring Stuff with Python”** by Al Sweigart: Ideal for beginners who want to learn how to automate repetitive tasks.

### YouTube Channels

- **Corey Schafer**: Detailed Python tutorials covering a wide range of topics.
- **Programming with Mosh**: Python tutorials for beginners and intermediate learners.

### Advanced Topics

- [Real Python](https://realpython.com/): A comprehensive site with tutorials for all skill levels.
- [Full Stack Python](https://www.fullstackpython.com/): Helps you learn how to develop and deploy Python web applications.

### Practice Platforms

- [LeetCode](https://leetcode.com/): Offers coding challenges to practice algorithmic thinking.
- [HackerRank](https://www.hackerrank.com/domains/tutorials/10-days-of-python): Provides Python challenges for all levels.

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
