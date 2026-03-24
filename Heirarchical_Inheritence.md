# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
```
class Details:
    def getName(self):
        self.name = input("Enter name: ")

    def getAge(self):
        while True:
            try:
                self.age = int(input("Enter age: "))
                break
            except ValueError:
                print("Please enter a valid number!")


class Employee(Details):
    def getEmployeeDetails(self):
        self.getName()
        self.getAge()
        self.employee_id = input("Enter employee ID: ")
        self.department = input("Enter department: ")

    def displayEmployee(self):
        print("\nEmployee Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Employee ID:", self.employee_id)
        print("Department:", self.department)


class Patient(Details):
    def getPatientDetails(self):
        self.getName()
        self.getAge()
        self.patient_id = input("Enter patient ID: ")
        self.disease = input("Enter disease: ")

    def displayPatient(self):
        print("\nPatient Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)


e = Employee()
p = Patient()

e.getEmployeeDetails()
e.displayEmployee()

p.getPatientDetails()
p.displayPatient()
```
## Sample Output
<img width="1054" height="427" alt="image" src="https://github.com/user-attachments/assets/51296aec-bcca-416e-92bc-6c764f181b51" />


## Result
Thus, the Python program demonstrating hierarchical inheritance to store and display Employee and Patient details was executed successfully, and the output was obtained.

