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

  # Example: For loop
  for i in range(5):
      print(i)  # Output: 0, 1, 2, 3, 4
  
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
  
  students = {"Alice": 85, "Bob": 90, "Charlie": 75}
  passed_students = {k: v for k, v in students.items() if v > 80}
  print(passed_students)  # Output: {'Alice': 85, 'Bob': 90}
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

## Contribution 🤝
Feel free to contribute by adding new examples, correcting errors, or enhancing explanations. Fork the repo and submit a **Pull Request (PR)**! 🚀

## License 📜
This project is licensed under the **MIT License**.

