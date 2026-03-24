# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method:
   - Initialize an instance variable `status` with the value `"Alive"`.
   - Print the value of `status`.
3. Define the `__del__` method:
   - Print a message indicating the object is being destroyed.
4. Outside the class:
   - Create an instance of the `Demo` class.
   - Delete the object using the `del` keyword.
## Program
```py
class Demo:
    def __init__(self):
        self.status = "Alive"
        print("Status:", self.status)

    def __del__(self):
        print("Object is being destroyed")
d = Demo()

del d
```
## 🧪 Output
<img width="564" height="388" alt="image" src="https://github.com/user-attachments/assets/ed8b25af-0ce1-4361-8a74-2b665885050b" />

## Result

Thus, the Python program demonstrating constructor and destructor was executed successfully, and the output obtained
