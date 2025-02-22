# Strings in Python

## What is a String?
A **string** is a sequence or collection of character data. It can include letters, numbers, or special characters. In Python, strings are immutable, meaning they cannot be changed after creation.

### String Representation
Strings must be enclosed in either **single quotes ('')** or **double quotes ("")**.

### Examples:
```python
"Anand"
"1233qeee"
"college"
"$wyw"
'abcd123'
```

---

## Finding the Type of a String
```python
a = "anand"
print(type(a))
```
**Output:**
```
<class 'str'>
```

### Checking if a Data Type is a String
```python
a = "anand"
print(isinstance(a, str))

b = 1233
print(isinstance(b, str))
```
**Output:**
```
True
False
```

---

# String Indexing

In Python, **string indexing** allows us to access individual characters using their position in the string.

- Indexing starts at **0** for the first character.
- Negative indexing starts from **-1** for the last character.

### Example:
```python
a = "COLLEGE"
print(a[0])  # C
print(a[5])  # G
print(a[-1]) # G
print(a[-6]) # C
```

If an index is out of range, Python raises an **IndexError**.
```python
print(a[10])
```
**Output:**
```
IndexError: string index out of range
```

---

# String Slicing

String slicing allows us to extract a part of a string using a range of indices.

### Syntax:
```python
variable_name[start_index:end_index:step]
```
- **start_index** (default: `0`)
- **end_index** (default: `len(variable_name) - 1`)
- **step** (default: `1`)

### Examples:
```python
a = "mystring"
print(a[1:4])   # 'yst'
print(a[:4])    # 'myst'
print(a[4:])    # 'ring'
print(a[1:5:2]) # 'yt'
print(a[::-1])  # Reverse the string
```

Negative slicing:
```python
print(a[-3:-1])  # 'in'
print(a[-4:-1])  # 'rin'
print(a[:-4])    # 'myst'
```

---

# String Methods

## Case Conversion Methods

### 1. `upper()`
Converts all characters in the string to uppercase.
```python
a = "Student"
print(a.upper())  # STUDENT
```

### 2. `lower()`
Converts all characters in the string to lowercase.
```python
a = "STUdent"
print(a.lower())  # student
```

### 3. `swapcase()`
Swaps uppercase characters to lowercase and vice versa.
```python
a = "STUDent"
print(a.swapcase())  # studENT
```

### 4. `title()`
Capitalizes the first letter of each word in the string.
```python
a = "hello world"
print(a.title())  # Hello World
```

### 5. `capitalize()`
Capitalizes only the first letter of the entire string.
```python
a = "hello world"
print(a.capitalize())  # Hello world
```

---

## Checking Content Methods

### 6. `isupper()`
Checks if all characters in the string are uppercase.
```python
a = "STUDENT"
print(a.isupper())  # True
```

### 7. `islower()`
Checks if all characters in the string are lowercase.
```python
a = "student"
print(a.islower())  # True
```

### 8. `isalpha()`
Checks if all characters in the string are alphabets.
```python
a = "Hello"
print(a.isalpha())  # True

b = "Hello123"
print(b.isalpha())  # False
```

### 9. `isdigit()`, `isnumeric()`, `isdecimal()`
Checks if all characters in the string are numbers.
```python
a = "123"
print(a.isdigit())   # True
print(a.isnumeric()) # True
print(a.isdecimal()) # True
```

### 10. `isalnum()`
Checks if all characters in the string are either alphabets or numbers.
```python
a = "Hello123"
print(a.isalnum())  # True

b = "Hello123!!"
print(b.isalnum())  # False
```

---

## Trimming and Formatting Methods

### 11. `strip()`, `lstrip()`, `rstrip()`
Removes leading/trailing spaces from a string.
```python
a = "   car   "
print(a.strip())  # 'car'
print(a.lstrip()) # 'car   '
print(a.rstrip()) # '   car'
```

### 12. `count()`
Counts occurrences of a substring within the string.
```python
a = "ababab"
print(a.count("ab"))  # 3
```

### 13. `join()`
Joins a list of strings using a separator.
```python
words = ['1', '2', '3']
print("-".join(words))  # '1-2-3'
```

### 14. `replace()`
Replaces occurrences of a substring with another substring.
```python
a = "ababab"
print(a.replace('a', 'c'))  # 'cbcbcb'
```

### 15. `find()`, `rfind()`, `index()`
Finds the first or last occurrence of a substring.
```python
a = "abcdefab"
print(a.find('a'))   # 0
print(a.rfind('a'))  # 6
print(a.index('a'))  # 0
```

---

# String Formatting

### Using `format()`
```python
name = "Anand"
print("My name is {}".format(name))
```

### Using f-strings
```python
a = 3
b = 5
s = a + b
print(f"Sum of {a} and {b} is {s}")
```
**Output:**
```
Sum of 3 and 5 is 8
```

# String Formatting in Python

String formatting is the process of inserting custom values or variables into a string. Python provides multiple ways to format strings efficiently. The two most commonly used methods are **`format()`** and **f-strings**.

---

## 1. Using `format()` Method
The `format()` method allows us to dynamically insert values into a string. This method replaces `{}` placeholders with the specified values in `format()`.

### Syntax:
```python
string.format(value1, value2, ...)
```

### Example 1: Basic Usage
```python
name = "Anand"
print("My name is {}".format(name))
```
**Output:**
```
My name is Anand
```

### Example 2: Formatting Multiple Values
```python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
sum = a + b
print("Sum of {} and {} is {}".format(a, b, sum))
```
#### Input:
```
2
3
```
#### Output:
```
Sum of 2 and 3 is 5
```

### Example 3: Using Positional Indexing
Python allows us to use indices inside `{}` to rearrange the values.
```python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
sum = a + b
print("Sum of {2} and {1} is {0}".format(sum, b, a))
```
#### Input:
```
2
3
```
#### Output:
```
Sum of 2 and 3 is 5
```

### Example 4: Using Named Placeholders
We can also use named placeholders inside `{}` and pass values as keyword arguments.
```python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
sum = a + b
print("Sum of {n1} and {n2} is {s}".format(s=sum, n1=b, n2=a))
```
#### Input:
```
2
3
```
#### Output:
```
Sum of 2 and 3 is 5
```

---

## 2. Using f-strings (Formatted String Literals)
Introduced in Python 3.6, **f-strings** provide a more readable and concise way to format strings. Instead of using `format()`, variables are directly inserted inside `{}` within an `f`-prefixed string.

### Syntax:
```python
f"string with {variable}"
```

### Example 1: Basic f-string Formatting
```python
a = 3
b = 5
s = a + b
print(f"Sum of {a} and {b} is {s}")
```
**Output:**
```
Sum of 3 and 5 is 8
```

### Example 2: Expressions Inside f-strings
We can include expressions inside `{}`.
```python
x = 10
y = 20
print(f"The product of {x} and {y} is {x * y}")
```
**Output:**
```
The product of 10 and 20 is 200
```

### Example 3: Formatting Numbers
f-strings support number formatting like specifying decimal places.
```python
pi = 3.14159
print(f"Value of Pi up to 2 decimal places: {pi:.2f}")
```
**Output:**
```
Value of Pi up to 2 decimal places: 3.14
```

### Example 4: Aligning Text with f-strings
We can align text using f-strings for better readability.
```python
name = "Python"
print(f"|{name:^10}|")  # Center align
print(f"|{name:<10}|")  # Left align
print(f"|{name:>10}|")  # Right align
```
**Output:**
```
|  Python  |
|Python    |
|    Python|
```

---

## Summary
| Method | Description |
|--------|-------------|
| `format()` | Uses `{}` placeholders to insert values dynamically. Supports positional and named arguments. |
| f-strings | More readable and efficient way to insert values inside a string. Allows expressions directly within `{}`. |

Both methods are useful in different scenarios, but **f-strings** are recommended for better readability and performance.

Now you have a solid understanding of string formatting in Python! 🚀



