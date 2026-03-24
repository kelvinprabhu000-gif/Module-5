# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
```py
class Calculation1:
    def Summation(self, a, b):
        return a + b


class Calculation2:
    def Subtraction(self, a, b):
        return a - b


class Derived(Calculation1, Calculation2):
    def Division(self, a, b):
        return a / b


a = int(input())
b = int(input())

d = Derived()

print("Sum:", d.Summation(a, b))
print("Subtraction:", d.Subtraction(a, b))

if b != 0:
    print("Division:", d.Division(a, b))
else:
    print("Division: Cannot divide by zero")
```
## Output Example
<img width="622" height="487" alt="image" src="https://github.com/user-attachments/assets/16c767b1-5986-4637-b217-435c95715150" />

### Result
Thus, the Python program demonstrating multiple inheritance for performing addition, subtraction, and division was executed successfully, and the output was obtained.
