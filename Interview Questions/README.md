## Basics Of Programming

### What is a Program?
A **program** is a collection of instructions that a computer can execute to solve a specific problem.  

### What is Programming?
**Programming** is the process of writing, testing, and maintaining a program to solve a specific problem.  

### What is a Programming Language?
A **programming language** is a formal language used to communicate with computers.  

### Types of Programming Languages
There are three types of programming languages:  

1. **Low-Level Languages** 🏩 – These languages are machine-friendly and can directly interact with hardware.  
   **Examples:** Binary Language, Assembly Language  

2. **Mid-Level Languages** ⚖️ – These languages are both machine-friendly and user-friendly.  
   **Examples:** C, C++  

3. **High-Level Languages** 🚀 – These languages are user-friendly and easy to read and write.  
   **Examples:** Python, Java, JavaScript

### What is compiler?
A **compiler** is a software that translates the high level language into low level language. It transaltes the entire code once and then executes. 

### What is interpreter?
A **interpreter** is a software that translates the high level language into low level language. It transalates code line by line and executes code line by line. 

### what is the difference between compiler and interpreter? 
| Feature | Compiler | Interpreter |  
|---------|---------|------------|  
| **Execution** | Translates the entire code at once and then runs | Translates and runs code line by line |  
| **Speed** | Faster (since the whole code is translated once) | Slower (since it translates line by line) |  
| **Error Handling** | Shows all errors at once | Stops at the first error and reports it immediately |  
| **Examples** | C, C++ (compiled languages) | Python, JavaScript (interpreted languages) |

## Variables

### 1. What is a Literal?

A **literal** is a representation of data or a fixed value in programming.

**Examples of Literals in Python:**

- **Numeric Literals** → `10`, `3.14`, `5+3j`
- **String Literals** → `"Hello"`, `'Python'`
- **Boolean Literals** → `True`, `False`

---

### 2. What is an Identifier?

An **identifier** is a name that refers to a memory location. It is used to identify programming elements like variables, functions, and classes.

✅ **Rules for Identifiers:**

- Can contain **letters (A-Z, a-z), digits (0-9), and underscores (\_) only**.
- Must **start with a letter or an underscore (\_), not a digit**.
- Cannot use **Python keywords** (`if`, `while`, `class`, etc.).
- **Case-sensitive** (`Name` and `name` are different).

---

### 3. What is a Variable?

A **variable** is an identifier that holds a value during program execution.

#### Example:

```python
age = 25  # 'age' is a variable storing an integer value
name = "Anand"  # 'name' is a variable storing a string
```

---

### 4. What is a Data Type?

A **data type** in programming is a classification of data that defines the type of data and determines the operations that can be performed on it without any errors.

For example:

```python
x = 10  # Integer data type
y = "Python"  # String data type
```

✅ **Purpose of Data Types:**

- Helps the interpreter understand how to store and manage values.



---

### 5. What are Data Types in Python?

Python has several built-in **data types**:

1. **Integer** (`int`)
2. **Float** (`float`)
3. **String** (`str`)
4. **Boolean** (`bool`)
5. **List** (`list`)
6. **Tuple** (`tuple`)
7. **Set** (`ser`)
8. **FrozenSet** (`frozenset`)
9. **Dictionary** (`dict`)

---

### Example Code with Different Data Types:

```python
# Numeric Types
x = 10  # int
y = 3.14  # float
z = 5 + 3j  # complex

# Sequence Types
name = "Anand"  # str
numbers = [1, 2, 3]  # list
values = (10, 20, 30)  # tuple

# Set and Dictionary
unique_numbers = {1, 2, 3}  # set
person = {"name": "Anand", "age": 25}  # dict

# Boolean and None
is_active = True  # bool
data = None  # NoneType
```




