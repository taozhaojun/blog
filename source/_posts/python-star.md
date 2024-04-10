---
title: Python `*` and `**` Operators
date: 2024-04-10 13:59:54
tags: python
---
Python features several powerful operators for unpacking collections and dictionaries, namely the `*` (asterisk) and `**` (double asterisk) operators. These operators are highly useful for function calls, handling variable numbers of arguments, and other situations requiring flexibility in how data is passed around.

<!-- more -->
## The `*` Operator (Asterisk)

The `*` operator is used to unpack iterable objects such as lists and tuples into individual elements. This is particularly useful in function calls and definitions.

### Example of Unpacking with `*`:

```python
def sum_numbers(a, b, c):
    return a + b + c

numbers = [1, 2, 3]
result = sum_numbers(*numbers)  # Unpacks the list into three separate arguments
print(result)  # Outputs: 6
```

### Using * to Accept Variable Number of Arguments:
You can also use * in a function definition to allow the function to accept any number of positional arguments.

```python
def print_numbers(*args):
    for number in args:
        print(number)

print_numbers(1, 2, 3, 4)  # Prints 1, 2, 3, 4 on separate lines
```
## The ** Operator (Double Asterisk)
The ** operator is used to unpack dictionaries into named arguments when calling functions. It can also be used to accept arbitrary keyword arguments in function definitions.

### Example of Unpacking with `**`:
```python
def describe_person(name, age):
    print(f"{name} is {age} years old.")

person_info = {'name': 'John', 'age': 25}
describe_person(**person_info)  # Unpacks the dictionary into named arguments
```
### Using ** to Accept Arbitrary Named Arguments:
In function definitions, ** can gather remaining keyword arguments as a dictionary, providing flexibility for passing optional or configuration parameters.
```python
def print_student_info(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

print_student_info(name="Jane", grade="A", age=22)  # Prints name: Jane, grade: A, age: 22
```
## Practical Applications
- Function Argument Flexibility: * and ** allow functions to handle varying numbers of arguments, making your code more flexible and adaptable.
- Simplifying API Integration: These operators can streamline the process of passing multiple parameters from stored data structures to API calls or other functions.
- Decorators and Higher-Order Functions: Commonly used in decorators, * and ** enable these functions to pass through any arguments the decorated function might accept.

Using these unpacking operators correctly can lead to cleaner, more efficient, and more readable Python code, especially in complex scenarios involving multiple function parameters or dynamic argument handling.