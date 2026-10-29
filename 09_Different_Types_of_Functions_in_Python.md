# Experiment 9: Different Types of Functions in Python

## Aim
To write a Python program demonstrating function definition, arguments, return values, scope, built-in functions, and lambda functions.

## Python Code

```python
# --- Program ---
# Function with arguments and no return value
def square_cube(num):
    Square = num ** 2
    Cube = num ** 3
    print("Square =", Square)
    print("Cube =", Cube, "\n")

N = int(input("Enter a number: "))
square_cube(N)

# Function with arguments and a return value
def check_even_odd(num):
    if num % 2 == 0:
        return "Even"
    return "Odd"

N = int(input("Enter a number: "))
Result = check_even_odd(N)
print(f"{N} is {Result}.\n")

# Function to calculate factorial
def factorial(num):
    Fact = 1
    for i in range(1, num + 1):
        Fact *= i
    return Fact

N = int(input("Enter a number: "))
if N < 0:
    print("Factorial is not defined for negative numbers.\n")
else:
    print("Factorial =", factorial(N), "\n")

# Function with default arguments
def simple_interest(principal, rate=5, time=1):
    SI = (principal * rate * time) / 100
    print("Simple Interest =", SI, "\n")

P = float(input("Enter Principal Amount: "))
simple_interest(P)

# Function using *args
def calculate_sum(*args):
    Total = sum(args)
    print("Sum =", Total)

calculate_sum(10, 20, 30)
calculate_sum(5, 15, 25, 35, 45)
print("\n")

# Function using **kwargs
def employee_details(**kwargs):
    print("Employee Details:")
    for key, value in kwargs.items():
        print(f"{key}: {value}")
    print("\n")

employee_details(
    Name="David",
    Age=19,
    Gender="Female",
    Department="Computer Science",
    Location="Seattle",
)

# Function returning multiple values
def calculate(values):
    Total = sum(values)
    Average = Total / len(values)
    Maximum = max(values)
    return Total, Average, Maximum

Numbers = [10, 20, 30, 40, 50]
S, Avg, Mx = calculate(Numbers)
print("Sum =", S)
print("Average =", Avg)
print("Maximum =", Mx, "\n")
```

## Theory
A function is a reusable block of code defined with `def`. Parameters are names in a function definition; arguments are values passed during a call. A function may return a result with `return`, or return `None` implicitly. Local variables are defined within a function, while global variables are defined at module level. Built-in functions include `len()`, `sum()`, and `max()`. A lambda expression creates a small anonymous function, such as `lambda x: x*x`. Functions improve modularity, reuse, and readability.

## Algorithm
1. Start the program.
2. Define a function with parameters.
3. Call the function with arguments and capture its returned result.
4. Demonstrate a function with no explicit return value if appropriate.
5. Use a built-in function on sample data.
6. Create and call a lambda function.
7. Display the outputs and stop.

## Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Define function(s)]
    B --> C[Call function with arguments]
    C --> D[Compute and return result]
    D --> E[Use built-in and lambda functions]
    E --> F[Display outputs]
    F --> G([Stop])
```

## Conclusion
The program demonstrates how Python functions support reusable code, parameter passing, returned values, and concise lambda expressions.

---
