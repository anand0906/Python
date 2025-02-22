### **Input in Python Programming**

In Python, the `input()`  is a built-in function which is used to take user input from the keyboard. 
It allows a program to take input from the user at runtime

---

## **1. Basic Syntax**
```python
input(prompt)
```
- `prompt`: (Optional) A string displayed to the user before taking input.
- The function returns the user input as a **string**.

---

## **2. Taking User Input**
### Example:
```python
name = input("Enter your name: ")
print("Hello,", name)
```
**Output:**
```
Enter your name: Anand
Hello, Anand
```
- The user enters `"Anand"`, and the program prints a greeting.

---

## **3. Converting Input Data Type**
Since `input()` returns a string, we often need to convert it to other data types.

### Example: Taking Integer Input
```python
age = int(input("Enter your age: "))
print("You will turn 100 in", 2024 + (100 - age))
```
**Output:**
```
Enter your age: 24
You will turn 100 in 2100
```
- `int(input())` converts the string input into an integer.

### Example: Taking Float Input
```python
height = float(input("Enter your height in meters: "))
print("Your height:", height)
```
**Output:**
```
Enter your height in meters: 1.75
Your height: 1.75
```

---

## **4. Taking Multiple Inputs**
### **Using `split()`**
To take multiple inputs in one line, use `.split()`.

```python
x, y = input("Enter two numbers: ").split()
print("First number:", x)
print("Second number:", y)
```
**Input:**
```
10 20
```
**Output:**
```
First number: 10
Second number: 20
```

### **Converting to Integers**
```python
a, b = map(int, input("Enter two numbers: ").split())
print("Sum:", a + b)
```
**Input:**
```
5 7
```
**Output:**
```
Sum: 12
```

---

## **5. Advanced: Reading Input from a File**
Python can also take input from a file using `sys.stdin`.

```python
import sys
data = sys.stdin.read()
print("File content:", data)
```

---

## **6. Handling Errors**
### Example: Handling Non-Numeric Input
```python
try:
    num = int(input("Enter a number: "))
    print("Square:", num ** 2)
except ValueError:
    print("Invalid input! Please enter a number.")
```
- If the user enters non-numeric input, it prints an error message.

---


