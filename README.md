# 30-Day Python Coding Challenge: From Basic to Advanced

Welcome to the **30-Day Python Coding Challenge**! 🚀 This challenge is designed to help you build a strong foundation in Python programming, covering essential concepts from basics to advanced topics. Each day, you'll solve a new problem, gain hands-on experience, and improve your coding skills.

## 📌 How to Use This Challenge
1. Read the daily problem statement.
2. Try to solve it on your own.
3. Compare your solution with the provided example.
4. Take notes and experiment with modifications.
5. Move on to the next day's challenge!

---

## 🏆 Challenge Breakdown

### **Day 1: Hello, World!**
**Task:** Write a Python program that prints "Hello, World!" to the console.
```python
print("Hello, World!")
```
**Concepts:** print() function, syntax basics.

### **Day 2: Variables and Data Types**
**Task:** Create variables of different data types (integer, float, string, boolean) and print them.
```python
age = 25
height = 1.75
name = "Alice"
is_student = True

print(f"Age: {age}, Type: {type(age)}")
print(f"Height: {height}, Type: {type(height)}")
print(f"Name: {name}, Type: {type(name)}")
print(f"Is Student: {is_student}, Type: {type(is_student)}")
```
**Concepts:** Dynamic typing, type() function, f-strings.

### **Day 3: Basic Arithmetic Operations**
**Task:** Perform basic arithmetic operations on two numbers.
```python
a = 10
b = 3

print(f"Addition: {a + b}")
print(f"Subtraction: {a - b}")
print(f"Multiplication: {a * b}")
print(f"Division: {a / b}")
print(f"Integer Division: {a // b}")
print(f"Modulus: {a % b}")
print(f"Exponentiation: {a ** b}")
```
**Concepts:** Operators, integer division, modulus, exponentiation.

### **Day 4: Conditional Statements**
**Task:** Check if a number is positive, negative, or zero.
```python
number = float(input("Enter a number: "))
if number > 0:
    print("The number is positive.")
elif number < 0:
    print("The number is negative.")
else:
    print("The number is zero.")
```
**Concepts:** if-elif-else, user input, float conversion.

### **Day 5: Loops - For Loop**
**Task:** Print the first 10 numbers of the Fibonacci sequence.
```python
def fibonacci(n):
    fib = [0, 1]
    for i in range(2, n):
        fib.append(fib[i-1] + fib[i-2])
    return fib

print(fibonacci(10))
```
**Concepts:** Loops, lists, range(), append().

### **Day 6: Loops - While Loop**
**Task:** Calculate the factorial of a number using a while loop.
```python
def factorial(n):
    result = 1
    while n > 0:
        result *= n
        n -= 1
    return result

number = int(input("Enter a number: "))
print(f"The factorial of {number} is {factorial(number)}")
```
**Concepts:** While loops, factorial calculation.

### **Day 7: Lists and List Comprehensions**
**Task:** Create a list of squares of even numbers from 0 to 20 using a list comprehension.
```python
squares = [x**2 for x in range(21) if x % 2 == 0]
print(squares)
```
**Concepts:** List comprehensions, range(), conditional filtering.

### **Day 8: Dictionaries**
**Task:** Count word occurrences in a given string using a dictionary.
```python
def word_frequency(sentence):
    words = sentence.lower().split()
    frequency = {}
    for word in words:
        frequency[word] = frequency.get(word, 0) + 1
    return frequency

sentence = "The quick brown fox jumps over the lazy dog"
print(word_frequency(sentence))
```
**Concepts:** Dictionaries, get() method, string methods.

### **Day 9: Functions and Default Arguments**
**Task:** Calculate the area of a rectangle with default values.
```python
def rectangle_area(length=1, width=1):
    return length * width

print(rectangle_area())
print(rectangle_area(5))
print(rectangle_area(4, 3))
print(rectangle_area(width=6))
```
**Concepts:** Functions, default arguments, keyword arguments.

### **Day 10: Error Handling**
**Task:** Handle division errors using try-except.
```python
try:
    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))
    result = num1 / num2
    print(f"The result of {num1} divided by {num2} is {result}")
except ValueError:
    print("Error: Please enter valid numbers.")
except ZeroDivisionError:
    print("Error: Cannot divide by zero.")
except Exception as e:
    print(f"An unexpected error occurred: {e}")
```
**Concepts:** Exception handling, multiple except blocks.

---

## 🔥 What’s Next?
The challenge continues with:
- File Handling (Reading/Writing Files)
- Object-Oriented Programming (Classes, Methods, Inheritance)
- Data Structures (Tuples, Sets, Stacks, Queues)
- Advanced Topics (Decorators, Generators, Lambda Functions)
- Web Scraping, APIs, and Database Interaction

Stay consistent and keep learning! Happy coding! 🚀🐍

---

## 📚 Resources
- [Python Official Documentation](https://docs.python.org/3/)
- [W3Schools Python Tutorial](https://www.w3schools.com/python/)
- [Real Python](https://realpython.com/)

## 🤝 Contribute
If you find any issues or have improvements, feel free to fork and contribute!


# Arithmetic and Relational Operators in Python

Python provides several arithmetic and relational operators for mathematical and logical computations. Below is a detailed explanation of each operator with examples.

## Arithmetic Operators

### 1. Addition (`+`)
Adds two numbers.

```python
# Addition Example
a = 10
b = 5
result = a + b  # 15
print(result)
```

### 2. Subtraction (`-`)
Subtracts the second number from the first.

```python
# Subtraction Example
result = a - b  # 5
print(result)
```

### 3. Multiplication (`*`)
Multiplies two numbers.

```python
# Multiplication Example
result = a * b  # 50
print(result)
```

### 4. Division (`/`)
Divides the first number by the second (returns a float).

```python
# Division Example
result = a / b  # 2.0
print(result)
```

### 5. Floor Division (`//`)
Divides and rounds down to the nearest integer.

```python
# Floor Division Example
result = a // b  # 2
print(result)
```

### 6. Modulus (`%`)
Returns the remainder of the division.

```python
# Modulus Example
result = a % b  # 0
print(result)
```

### 7. Exponentiation (`**`)
Raises the first number to the power of the second.

```python
# Exponentiation Example
result = a ** b  # 10^5 = 100000
print(result)
```

## Relational Operators
Relational operators compare values and return a Boolean result (True or False).

### 1. Equal to (`==`)
Checks if two values are equal.

```python
# Equal to Example
print(a == b)  # False
```

### 2. Not Equal to (`!=`)
Checks if two values are not equal.

```python
# Not Equal to Example
print(a != b)  # True
```

### 3. Greater than (`>`)
Checks if the left operand is greater than the right.

```python
# Greater than Example
print(a > b)  # True
```

### 4. Less than (`<`)
Checks if the left operand is less than the right.

```python
# Less than Example
print(a < b)  # False
```

### 5. Greater than or equal to (`>=`)
Checks if the left operand is greater than or equal to the right.

```python
# Greater than or equal to Example
print(a >= b)  # True
```

### 6. Less than or equal to (`<=`)
Checks if the left operand is less than or equal to the right.

```python
# Less than or equal to Example
print(a <= b)  # False
```

### 📌 Notes:
- Relational operators return `True` or `False` based on the condition.
- They are commonly used in decision-making statements like `if` conditions.
- They help in sorting and filtering data.

Happy Coding! 🚀




# Python Logical Operators & Type Conversion

This repository demonstrates the use of logical operators and type conversion in Python. Both topics are essential for writing clear and effective code.

## Logical Operators

Logical operators in Python are used to perform operations on Boolean values (`True` or `False`). There are three main logical operators:

### 1️⃣ `and` (Logical AND)
**Description:** Returns `True` only if both conditions are `True`. If either or both conditions are `False`, it returns `False`.

#### Syntax:
```python
a and b
```
#### Example:
```python
x = True
y = False
print(x and y)  # Output: False

print(5 > 3 and 10 > 2)  # Output: True
print(5 > 3 and 10 < 2)  # Output: False
```

### 2️⃣ `or` (Logical OR)
**Description:** Returns `True` if at least one condition is `True`. Returns `False` only if both conditions are `False`.

#### Syntax:
```python
a or b
```
#### Example:
```python
x = True
y = False
print(x or y)  # Output: True

print(5 > 3 or 10 < 2)  # Output: True
print(5 < 3 or 10 < 2)  # Output: False
```

### 3️⃣ `not` (Logical NOT)
**Description:** Reverses the Boolean value. If the condition is `True`, it returns `False`, and vice versa.

#### Syntax:
```python
not a
```
#### Example:
```python
x = True
print(not x)  # Output: False

print(not (5 > 3))  # Output: False
print(not (5 < 3))  # Output: True
```

### Example Using All Logical Operators
```python
a = 10
b = 5

print("a > 5 and b < 10:", (a > 5) and (b < 10))   # True (Both conditions are True)
print("a < 5 or b == 5:", (a < 5) or (b == 5))       # True (One condition is True)
print("not (a == 10):", not (a == 10))               # False (Reverses True to False)
```

### Truth Table for Logical Operators
| A (Condition 1) | B (Condition 2) | A and B | A or B | not A |
|-----------------|-----------------|---------|--------|-------|
| True           | True           | True    | True   | False |
| True           | False          | False   | True   | False |
| False          | True           | False   | True   | True  |
| False          | False          | False   | False  | True  |

## Use Cases

### Conditional Statements
Use logical operators in `if-else` conditions.
```python
age = 20
if age > 18 and age < 30:
    print("Eligible for the program.")  # Output: Eligible for the program.
```

### Checking Multiple Conditions
```python
username = "admin"
password = "1234"

if username == "admin" and password == "1234":
    print("Access Granted!")  # Output: Access Granted!
else:
    print("Access Denied!")
```

### Boolean Toggling
```python
is_logged_in = False
is_logged_in = not is_logged_in  # Now becomes True
print(is_logged_in)  # Output: True
```

---

## Type Conversion in Python

Type conversion refers to converting a variable from one data type to another. Python provides several built-in functions for this purpose.

### Common Type Conversion Functions

#### `int()`: Converts a value to an integer.
```python
num_str = "100"
num_int = int(num_str)  # 100 as an integer
print(num_int, type(num_int))
```

#### `float()`: Converts a value to a floating-point number.
```python
num_str = "3.14"
num_float = float(num_str)  # 3.14 as a float
print(num_float, type(num_float))
```

#### `str()`: Converts a value to a string.
```python
num = 100
num_str = str(num)  # "100" as a string
print(num_str, type(num_str))
```

#### `list()`: Converts an iterable (like a tuple) into a list.
```python
tup = (1, 2, 3)
lst = list(tup)  # [1, 2, 3] as a list
print(lst, type(lst))
```

#### `tuple()`: Converts an iterable (like a list) into a tuple.
```python
lst = [1, 2, 3]
tup = tuple(lst)  # (1, 2, 3) as a tuple
print(tup, type(tup))
```

### Example: Combining Type Conversion with Logical Operations
```python
# Convert string to int and use in a logical condition
num_str = "20"
num = int(num_str)  # Convert string to int

if num > 10 and num < 30:
    print("The number is between 10 and 30.")  # Output: The number is between 10 and 30.
else:
    print("The number is out of range.")

# Converting a float to int for further calculation
pi = 3.14159
pi_int = int(pi)  # Converts to 3 (truncates the decimal)
print("Integer value of pi:", pi_int)
```

## Conclusion

- **Logical Operators:** `and`, `or`, and `not` are essential for making decisions in your Python code.
- **Type Conversion:** Functions like `int()`, `float()`, `str()`, `list()`, and `tuple()` enable you to convert data types, making it easier to manipulate and compare data.

🚀 **Happy Coding!**

