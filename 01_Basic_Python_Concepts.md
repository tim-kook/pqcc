# Experiment 1: Basic Python Concepts: Input, Output, Variables, Keywords, and Identifiers

## Aim
To write and execute a Python program demonstrating input, output, variables, keywords, and identifiers.

## Python Code

```python
# --- Hello World ---
print("Hello World!\n")

# --- Swap variables ---
A = 5
B = 10
print("Before Swap:\nA =", A, "\nB =", B)
A, B = B, A
print("\nAfter Swap:\nA =", A, "\nB =", B, "\n")

# --- Personal information output ---
Name = "David"
Age = 19
Gender = "Female"
Course = "Computer Science"
Address = "Seattle"
print("Name:", Name)
print("Age:", Age)
print("Gender:", Gender)
print("Course:", Course)
print("Address:", Address, "\n")

# --- Personal information using input ---
Name_Input = input("Enter Name: ")
Age_Input = input("Enter Age: ")
Course_Input = input("Enter Course: ")
Address_Input = input("Enter Address: ")
print("\nName:", Name_Input)
print("Age:", Age_Input)
print("Course:", Course_Input)
print("Address:", Address_Input, "\n")
```

## Theory
Python is a high-level, interpreted programming language. `input()` accepts data from the user as text, while `print()` displays output. A variable is a name that refers to a value; Python determines its type dynamically. An identifier is a name used for variables, functions, and other objects. Identifiers may contain letters, digits, and underscores, cannot begin with a digit, and cannot be a reserved keyword. Keywords such as `if`, `for`, `def`, and `class` have predefined meanings in Python. Comments begin with `#`.

## Algorithm
1. Start the program.
2. Display a prompt and accept input from the user.
3. Store the input in a variable and convert it to the required type if necessary.
4. Create additional variables to demonstrate assignment.
5. Display the values using `print()`.
6. Optionally display Python keywords using the `keyword` module.
7. Stop the program.

## Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Accept user input/]
    B --> C[Store values in variables]
    C --> D[Display values using print()]
    D --> E[Optionally display keywords]
    E --> F([Stop])
```

## Conclusion
The program demonstrates Python input/output, variable assignment, identifiers, and the role of reserved keywords.

---
