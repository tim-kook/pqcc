# Experiment 13: Tuple Operations: Accessing, Concatenation, Slicing, and Deleting

## Aim
To demonstrate accessing, concatenating, slicing, and deleting a tuple in Python.

## Python Code

```python
# --- Program ---
# Accessing
print("--- Tuple Accessing ---")
A = (10, 20, 30, 40)
print("Element at index 3:", A[3], "\n")

# Concatenation
print("--- Tuple Concatenation ---")
A = (20, 30, 40, 59, 90)
B = (34, 56, 60, 79, 90)
C = A + B
print("The new tuple is:", C, "\n")

# Slicing
print("--- Tuple Slicing ---")
A = (20, 30, 40, 59, 90)
print("Sliced Tuple:", A[:4], "\n")

# Sum and average
print("--- Sum and Average ---")
T = (10, 20, 30, 40, 50)
Total = sum(T)
Average = Total / len(T)
print("Sum =", Total)
print("Average =", Average, "\n")

# Length of tuple
print("--- Length Calculation ---")
T = (10, 20, 30, 40, 50)
Count = 0
for i in T:
    Count += 1
print("Length of tuple =", Count, "\n")

# Search element
print("--- Search Element ---")
T = (10, 20, 30, 40, 50)
Element = int(input("Enter element to search: "))
if Element in T:
    print("Element exists in the tuple.\n")
else:
    print("Element does not exist.\n")

# Extract even and odd numbers
print("--- Even and Odd Extraction ---")
T = (18, 15, 22, 37, 48, 51, 64)
print("Even numbers:")
for i in T:
    if i % 2 == 0:
        print(i, end=" ")
print("\nOdd numbers:")
for i in T:
    if i % 2 != 0:
        print(i, end=" ")
print("\n\n")

# Remove duplicates while preserving order
print("--- Remove Duplicates ---")
T = (10, 20, 10, 30, 40, 20, 50)
New_Tuple = tuple(dict.fromkeys(T))
print("Original tuple:", T)
print("Tuple after removing duplicates:", New_Tuple, "\n")

# Second-smallest and second-largest distinct values
print("--- Second Smallest and Largest ---")
T = (10, 50, 30, 20, 40)
Values = sorted(set(T))
if len(Values) < 2:
    raise ValueError("At least two distinct values are required")
print("Second smallest =", Values[1])
print("Second largest =", Values[-2], "\n")

# Reverse tuple
print("--- Reverse Tuple ---")
T = (10, 20, 30, 40, 50)
Rev = ()
for i in T:
    Rev = (i,) + Rev
print("Original tuple:", T)
print("Reversed tuple:", Rev, "\n")

# Delete tuple name
print("--- Tuple Deletion ---")
A = (1, 2, 3, 4, 5, 6, 7, 8, 9, 0)
print("Before Deletion:", A)
del A
print("Tuple variable deleted")
```

## Theory
A tuple is an ordered collection that is generally immutable after creation. Elements can be accessed by index and a portion can be selected with slicing. Concatenation with `+` creates a new tuple. Individual tuple elements cannot be reassigned or removed, but the entire tuple variable can be deleted with `del`. A one-element tuple requires a trailing comma, for example `(5,)`.

## Algorithm
1. Start the program.
2. Create two tuples with sample values.
3. Access and display an element using its index.
4. Concatenate the tuples and display the result.
5. Slice a portion of a tuple and display it.
6. Demonstrate deleting the tuple variable with `del` after all required operations.
7. Stop.

## Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Create tuple(s)]
    B --> C[Access element]
    C --> D[Concatenate tuples]
    D --> E[Slice tuple]
    E --> F[Display results]
    F --> G[Delete tuple variable if required]
    G --> H([Stop])
```

## Conclusion
The program demonstrates tuple access, concatenation, and slicing, and shows that deletion applies to the tuple variable rather than individual tuple elements.

---
