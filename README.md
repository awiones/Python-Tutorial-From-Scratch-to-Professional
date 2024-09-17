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

