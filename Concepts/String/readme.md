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

