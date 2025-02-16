# Python_Revision

# Python Complete Guide 📘

## Overview 🚀
This repository contains a **comprehensive guide to Python**, covering topics from **basic syntax** to **advanced concepts** like object-oriented programming, iterators, decorators, and more. The guide is structured for beginners and intermediate developers to gain a strong understanding of Python programming.

## Table of Contents 📑

1. [Python Basics](#python-basics)
2. [Control Flow](#control-flow)
3. [Data Structures](#data-structures)
4. [Functions](#functions)
5. [Modules & Standard Library](#modules--standard-library)
6. [File Handling & Exception Handling](#file-handling--exception-handling)
7. [Object-Oriented Programming (OOP)](#object-oriented-programming-oop)
8. [Advanced Python Concepts](#advanced-python-concepts)
9. [Iterators & Generators](#iterators--generators)
10. [Decorators](#decorators)
11. [Operator Overloading](#operator-overloading)

---

## Python Basics 🐍
- Introduction to Python syntax & semantics
- Variables and data types
- Operators and expressions
- Example:
  ```python
  # Case Sensitivity in Python
  name = "Ritesh"  # Variable with lowercase
  Name = "Mesh"   # Different variable due to case sensitivity
  print(name)  # Output: Ritesh
  print(Name)  # Output: Mesh
  ```

## Control Flow 🔄
- Conditional statements (`if`, `if-else`, `elif`)
- Looping structures (`for`, `while`)
- Loop control (`break`, `continue`)
- Example:
  ```python
  # Example: If-else statement
  num = 10
  if num > 0:
      print("Positive number")  # This will execute
  else:
      print("Negative number")
  ```
  
  ```python
  # Example: For loop
  for i in range(5):
      print(i)  # Output: 0, 1, 2, 3, 4
  ```
  
  ```python
  # Example: While loop with break and continue
  count = 0
  while count < 5:
      if count == 2:
          count += 1
          continue  # Skip printing when count is 2
      print(count)
      count += 1
  ```

## Data Structures 📊
- Lists, Tuples, Sets, Dictionaries
- List & Dictionary comprehension
- Example:
  ```python
  # Example: List & Dictionary comprehension
  squares = [x**2 for x in range(5)]  # List comprehension
  print(squares)  # Output: [0, 1, 4, 9, 16]
  ```

## Functions 🔧
- Defining and calling functions
- Lambda functions
- Example:
  ```python
  # Example: Function definition
  def greet(name):
      return "Hello, " + name
  
  print(greet("Alice"))  # Output: Hello, Alice
  ```

## Modules & Standard Library 📦
- Importing built-in & external modules
- Example:
  ```python
  # Example: Using built-in modules
  import math, random, os, datetime
  print(math.sqrt(16))  # Output: 4.0
  print(random.randint(1, 10))  # Output: Random number from 1 to 10
  print(os.getcwd())  # Output: Current working directory
  print(datetime.datetime.now())  # Output: Current date and time
  ```

## File Handling & Exception Handling 📂⚠️
- Reading & writing files (`open()`, `with` statement)
- Handling exceptions (`try-except` blocks)
- Example:
  ```python
  # Example: Reading a file and handling exceptions
  try:
      with open("example.txt", "r") as file:
          content = file.read()
          print(content)
  except FileNotFoundError:
      print("File not found!")
  ```

## Object-Oriented Programming (OOP) 🏛️
- Classes and objects
- Inheritance & Polymorphism
- Encapsulation & Abstraction
- Example:
  ```python
  # Example: Creating a class and using inheritance
  class Animal:
      def speak(self):
          print("Animal speaks")
  
  class Dog(Animal):
      def speak(self):
          print("Dog barks")
  
  dog = Dog()
  dog.speak()  # Output: Dog barks
  ```

## Iterators & Generators 🔄⚡
- Iterators: Objects that allow sequential access to elements.
- Generators: Functions using `yield` to return values lazily.
- Example:
  ```python
  # Example: Generator function
  def generate_numbers():
      for i in range(5):
          yield i
  
  gen = generate_numbers()
  for num in gen:
      print(num)  # Output: 0, 1, 2, 3, 4
  ```

## Decorators 🏗️
- Functions that modify other functions.
- Example:
  ```python
  # Example: Using a decorator
  def decorator_function(original_function):
      def wrapper_function():
          print("Wrapper executed before {}".format(original_function.__name__))
          return original_function()
      return wrapper_function
  
  @decorator_function
  def say_hello():
      print("Hello!")
  
  say_hello()
  ```

## Operator Overloading ➕➖
- Customizing how operators work with user-defined objects.
- Example:
  ```python
  # Example: Operator overloading
  class Point:
      def __init__(self, x, y):
          self.x = x
          self.y = y
      def __add__(self, other):
          return Point(self.x + other.x, self.y + other.y)
  
  p1 = Point(2, 3)
  p2 = Point(4, 5)
  result = p1 + p2
  print(result.x, result.y)  # Output: 6, 8
  ```

---

## Contribution 🤝
Feel free to contribute by adding new examples, correcting errors, or enhancing explanations. Fork the repo and submit a **Pull Request (PR)**! 🚀

## License 📜
This project is licensed under the **MIT License**.

