# # Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.

## 🧠 Algorithm
1. **Get user input**: Accept the student's name from the user.
2. **Define the class**: Create a class `Student` with a default constructor (`__init__`).
3. **Default Constructor**: In the constructor, assign the user input (student name) to an instance variable `self.a`.
4. **Display Message**: Define a method `show` that prints "This is non-parameterized constructor" and a welcome message with the student’s name.
5. **Execute the Program**: Instantiate the `Student` class and call the `show` method.

## 🧾 Program
```py
class Student:
    def __init__(self):
        self.a = input("Enter student name: ")

    def show(self):
        print("This is non-parameterized constructor")
        print("Welcome", self.a)

s = Student()
s.show()
```
## Output
<img width="653" height="482" alt="image" src="https://github.com/user-attachments/assets/b7657a69-3274-4665-bc30-284542ccf53d" />

## Result
Thus, the Python program to create a Student class with a default constructor and display a welcome message was executed successfully, and the output was obtained.


