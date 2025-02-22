# Python Data Types

## What is a Data Type?
**Data type** in programming is a classification of data that specifies the type of data and which type of operations that can be applied to it without raising any error.

## Data Types in Python
Python provides several built-in data types:

### Primary Data Types:
1. **int** (Integer)
2. **float** (Floating-point Number)
3. **str** (String)
4. **list** (List)
5. **tuple** (Tuple)
6. **dict** (Dictionary)
7. **set** (Set)
8. **frozenset** (Frozen Set)
9. **bool** (Boolean)

### Additional Data Types:
10. **complex** (Complex Numbers)
11. **bytes** (Bytes)
12. **bytearray** (Byte Array)

---

## 1. Integer (`int`)
- Represents numerical values (positive, negative, or zero)
- Can be of any length

### Examples:
```python
1
1000
20000000
-100000000
0
```

### Program to Find the Type of Data:
```python
a = 2
print(type(a))
```
**Output:**
```
<class 'int'>
```

### Program to Check if a Given Data is an Integer:
```python
a = 2
print(isinstance(a, int))

name = "Anand"
print(isinstance(name, int))
```
**Output:**
```
True
False
```

---

## 2. Floating-Point Number (`float`)
- Represents decimal numbers
- Can be positive or negative
- Must contain a decimal point
- Contains only digits (0-9) and one decimal point (`.`)
- Accurate up to 15 decimal places

### Examples:
```python
1.2
1.333
123.444
-1.34
0.0
```

### Program to Find the Type of Data:
```python
test = 3.14
result = type(test)
print(result)
```
**Output:**
```
<class 'float'>
```

### Program to Check if a Given Data is a Float:
```python
test = 1.23
a = isinstance(test, float)
print(a)

te = 2
print(isinstance(te, float))
```
**Output:**
```
True
False
```

### Special Cases of Float Representation:
```python
1.2e4  # 1.2 * 10^4
1.3E4  # 1.3 * 10^4
1.2e-4 # 1.2 * 10^-4
1.5E-4 # 1.5 * 10^-4
```

### Maximum and Minimum Values of Float:
```python
print(1.79e308)  # Maximum float value
print(1.8e308)   # Beyond max, results in 'inf'
```
**Output:**
```
1.79e+308
inf
```

```python
print(5e-324)  # Minimum float value
print(5e-325)  # Beyond min, results in 0.0
```
**Output:**
```
5e-324
0.0
```

---

## 3. Strings (`str`)
- A sequence or collection of characters
- Can contain letters, numbers, or special characters
- Defined using single (`'`) or double (`"`) quotes
- Strings are immutable (cannot be changed after creation)

### Examples:
```python
"Anand"
"1233qeee"
"college"
"$wyw"
'abcd123'
```

### Program to Find the Type of Data:
```python
a = "anand"
print(type(a))
```
**Output:**
```
<class 'str'>
```

### Program to Check if a Given Data is a String:
```python
a = "anand"
print(isinstance(a, str))

a = 1233
print(isinstance(a, str))
```
**Output:**
```
True
False
```

### Type Conversion:
#### Convert Integer to String:
```python
a = 2
print(a, type(a))
a = str(a)
print(a, type(a))
```
**Output:**
```
2 <class 'int'>
2 <class 'str'>
```

#### Convert Float to String:
```python
a = 10.4
print(a, type(a))
a = str(a)
print(a, type(a))
```
**Output:**
```
10.4 <class 'float'>
10.4 <class 'str'>
```


