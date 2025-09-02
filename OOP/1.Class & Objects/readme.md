

## Table of Contents
1. [What is Programming?](#what-is-programming)
2. [Programming Paradigms](#programming-paradigms)
3. [Object-Oriented Programming (OOP)](#object-oriented-programming-oop)
4. [Classes and Objects](#classes-and-objects)
5. [Variables in OOP](#variables-in-oop)
6. [Methods in OOP](#methods-in-oop)
7. [Special Methods (Dunder Methods)](#special-methods-dunder-methods)
8. [Constructor and Destructor](#constructor-and-destructor)

---

## What is Programming?

**Programming** is the process of writing instructions (code) to tell a computer how to solve a specific problem or perform a particular task.

### Real-World Example:
Think of programming like writing a recipe:
- **Problem**: Making a cake
- **Programming**: Writing step-by-step instructions for the baker
- **Computer**: The baker who follows the recipe exactly

---

## Programming Paradigms

**Programming Paradigm** is an approach, method, or way of solving problems through programming.

### Types of Programming Paradigms:

| Paradigm | Focus | Example |
|----------|-------|---------|
| **Imperative** | How to do something | Step-by-step instructions |
| **Declarative** | What to achieve | SQL queries |
| **Procedural** | Functions and procedures | C programming |
| **Functional** | Mathematical functions | Haskell, Lisp |
| **Object-Oriented** | Objects and classes | Java, Python, C++ |

### Limitations of Procedural Programming:
- ❌ **Can't solve complex real-world problems effectively**
- ❌ **High complexity** due to numerous functions
- ❌ **Low security** - no access control mechanisms
- ❌ **Global data issues** - difficult to track data changes

---

## Object-Oriented Programming (OOP)

**OOP** is a programming paradigm that focuses on creating objects that contain both **data (properties)** and **functions (methods)** bundled together.

### Key Benefits:
- ✅ **Solves real-world problems** naturally
- ✅ **Lower complexity** through organization
- ✅ **Higher security** with access specifiers
- ✅ **Better data management** through encapsulation

### Real-World Analogy:
Think of a **Car**:
- **Properties**: Color, model, speed, fuel level
- **Methods**: Start engine, accelerate, brake, turn

---

## Classes and Objects

### Class
A **class** is like a blueprint, template, or mold for creating objects.

#### Multiple Definitions:
- **Blueprint**: A plan showing how to build something
- **Template**: A pre-designed format
- **Mold**: A shape used to create multiple identical items
- **Definition**: Contains properties and methods to create objects

### Object
An **object** is a real-world entity created from a class that has both properties and behaviors.

#### Key Points:
- **Instance of a class**: A specific example created from the blueprint
- **Physical existence**: Actual implementation of the class
- **Unique identity**: Each object has its own memory space

### Real-World Examples:

| Class | Objects |
|-------|---------|
| **Human** | John, Mary, David |
| **Vehicle** | Toyota Camry, Honda Civic, BMW X5 |
| **Animal** | Dog named Buddy, Cat named Whiskers |
| **Phone** | iPhone 14, Samsung Galaxy S23 |

### Class Definition Syntax:

```python
class ClassName:
    """
    Optional docstring to describe the class
    """
    # Properties/variables
    # Methods/functions
```

### Example:

```python
class Human:
    """
    This class represents a human being
    """
    pass

# Creating an object
person1 = Human()
print(person1.__doc__)  # Output: This class represents a human being
```

---

## Variables in OOP

### 1. Instance Variables (Object-level)

**Definition**: Variables whose values vary from object to object. Each object has its own copy.

#### Characteristics:
- ✅ **Unique to each object**
- ✅ **Created using object reference**
- ✅ **Accessed only by respective object**

#### Creating Instance Variables:

```python
class Student:
    def __init__(self):
        pass

# Creating objects
student1 = Student()
student2 = Student()

# Adding instance variables
student1.name = "Alice"
student1.age = 20
student1.grade = "A"

student2.name = "Bob"
student2.age = 19
student2.grade = "B"

print(vars(student1))  # {'name': 'Alice', 'age': 20, 'grade': 'A'}
print(vars(student2))  # {'name': 'Bob', 'age': 19, 'grade': 'B'}
```

#### Real-World Example:

```python
class Car:
    def __init__(self):
        pass

# Different cars with different properties
car1 = Car()
car1.brand = "Toyota"
car1.color = "Red"
car1.year = 2023

car2 = Car()
car2.brand = "Honda"
car2.color = "Blue"
car2.year = 2022

print(f"{car1.brand} car is {car1.color}")  # Toyota car is Red
print(f"{car2.brand} car is {car2.color}")  # Honda car is Blue
```

### 2. Static Variables (Class-level)

**Definition**: Variables that are common to all objects of a class. All objects share the same copy.

#### Characteristics:
- ✅ **Shared by all objects**
- ✅ **Created using class reference**
- ✅ **Memory efficient**

#### Creating Static Variables:

```python
class Student:
    # Static variable - same for all students
    college = "ABC University"
    
    def __init__(self):
        pass

# All objects share the same college name
student1 = Student()
student2 = Student()

print(Student.college)    # ABC University
print(student1.college)   # ABC University
print(student2.college)   # ABC University
```

#### Real-World Example:

```python
class Employee:
    # Static variables - same for all employees
    company_name = "TechCorp"
    company_address = "123 Tech Street"
    
    def __init__(self, name, employee_id):
        # Instance variables - unique for each employee
        self.name = name
        self.employee_id = employee_id

emp1 = Employee("John", "E001")
emp2 = Employee("Sarah", "E002")

print(f"Both work at: {Employee.company_name}")
print(f"{emp1.name} - ID: {emp1.employee_id}")
print(f"{emp2.name} - ID: {emp2.employee_id}")
```

### 3. Local Variables (Method-level)

**Definition**: Temporary variables defined inside methods that exist only during method execution.

#### Characteristics:
- ✅ **Exist only during method execution**
- ✅ **Destroyed after method completes**
- ✅ **Cannot be accessed outside the method**

```python
class Calculator:
    def add_numbers(self):
        # Local variables
        a = 10
        b = 20
        result = a + b  # Local variable
        print(f"Sum: {result}")

calc = Calculator()
calc.add_numbers()  # Sum: 30
# print(calc.a)  # This would cause an error - 'a' doesn't exist outside method
```

---

## Methods in OOP

### 1. Instance Methods

**Definition**: Methods that are bound to object instances and can access instance variables.

#### Characteristics:
- ✅ **Must have `self` as first parameter**
- ✅ **Called using object reference**
- ✅ **Can access instance and static variables**

```python
class BankAccount:
    def __init__(self, account_holder, balance):
        self.account_holder = account_holder
        self.balance = balance
    
    def deposit(self, amount):  # Instance method
        self.balance += amount
        print(f"Deposited ${amount}. New balance: ${self.balance}")
    
    def withdraw(self, amount):  # Instance method
        if amount <= self.balance:
            self.balance -= amount
            print(f"Withdrew ${amount}. Remaining balance: ${self.balance}")
        else:
            print("Insufficient funds!")

# Usage
account = BankAccount("John Doe", 1000)
account.deposit(500)   # Deposited $500. New balance: $1500
account.withdraw(200)  # Withdrew $200. Remaining balance: $1300
```

### 2. Class Methods

**Definition**: Methods that are bound to the class rather than instances, using `@classmethod` decorator.

#### Characteristics:
- ✅ **Must have `cls` as first parameter**
- ✅ **Can be called using class or object reference**
- ✅ **Can access only static variables**

```python
class University:
    total_students = 0  # Static variable
    university_name = "ABC University"
    
    def __init__(self, student_name):
        self.student_name = student_name
        University.total_students += 1
    
    @classmethod
    def get_total_students(cls):  # Class method
        return f"Total students in {cls.university_name}: {cls.total_students}"
    
    @classmethod
    def change_university_name(cls, new_name):  # Class method
        cls.university_name = new_name

# Usage
student1 = University("Alice")
student2 = University("Bob")

print(University.get_total_students())  # Total students in ABC University: 2
University.change_university_name("XYZ University")
print(University.get_total_students())  # Total students in XYZ University: 2
```

### 3. Static Methods

**Definition**: Methods that are independent of both class and object, using `@staticmethod` decorator.

#### Characteristics:
- ✅ **No automatic reference parameter**
- ✅ **Can be called using class or object reference**
- ✅ **Cannot access instance or class variables directly**

```python
class MathUtils:
    @staticmethod
    def add(a, b):  # Static method
        return a + b
    
    @staticmethod
    def multiply(a, b):  # Static method
        return a * b
    
    @staticmethod
    def is_even(number):  # Static method
        return number % 2 == 0

# Usage - can call with class or object
result1 = MathUtils.add(5, 3)        # 8
result2 = MathUtils.multiply(4, 6)   # 24

obj = MathUtils()
result3 = obj.is_even(10)            # True
```

---

## Special Methods (Dunder Methods)

**Dunder Methods** (Double Underscore) are special methods that start and end with double underscores (`__`). They are automatically called when specific operations are performed on objects.

### Common Dunder Methods:

| Method | Purpose | When Called |
|--------|---------|-------------|
| `__init__` | Constructor | Object creation |
| `__del__` | Destructor | Object deletion |
| `__str__` | String representation | `print(obj)` or `str(obj)` |
| `__len__` | Length | `len(obj)` |
| `__add__` | Addition | `obj1 + obj2` |

### Example:

```python
class Book:
    def __init__(self, title, pages):
        self.title = title
        self.pages = pages
        print(f"Book '{self.title}' created!")
    
    def __str__(self):
        return f"Book: {self.title} ({self.pages} pages)"
    
    def __len__(self):
        return self.pages
    
    def __del__(self):
        print(f"Book '{self.title}' destroyed!")

# Usage
book = Book("Python Programming", 300)  # Book 'Python Programming' created!
print(book)        # Book: Python Programming (300 pages)
print(len(book))   # 300
del book          # Book 'Python Programming' destroyed!
```

---

## Constructor and Destructor

### Constructor (`__init__`)

**Purpose**: Automatically initialize object properties when an object is created.

#### Key Points:
- ✅ **Called automatically** during object creation
- ✅ **Called only once** per object
- ✅ **Used to set initial values**

#### Real-World Example - Smartphone:

```python
class Smartphone:
    def __init__(self, brand, model, storage, battery_percentage=100):
        # Instance variables initialized in constructor
        self.brand = brand
        self.model = model
        self.storage = storage
        self.battery_percentage = battery_percentage
        self.is_on = False
        print(f"{brand} {model} smartphone created!")
    
    def power_on(self):
        self.is_on = True
        print(f"{self.brand} {self.model} is now ON")
    
    def use_app(self, app_name, battery_drain=5):
        if self.is_on and self.battery_percentage > 0:
            self.battery_percentage -= battery_drain
            print(f"Using {app_name}. Battery: {self.battery_percentage}%")
        else:
            print("Phone is off or battery dead!")

# Creating smartphone objects
iphone = Smartphone("Apple", "iPhone 15", "128GB")
# Output: Apple iPhone 15 smartphone created!

android = Smartphone("Samsung", "Galaxy S24", "256GB", 80)
# Output: Samsung Galaxy S24 smartphone created!

# Using the objects
iphone.power_on()           # Apple iPhone 15 is now ON
iphone.use_app("Instagram") # Using Instagram. Battery: 95%
```

### Constructor with Parameters:

```python
class Restaurant:
    def __init__(self, name, cuisine_type, rating=0):
        self.name = name
        self.cuisine_type = cuisine_type
        self.rating = rating
        self.is_open = False
        self.menu_items = []
        print(f"Restaurant '{self.name}' established!")
    
    def add_menu_item(self, item, price):
        self.menu_items.append({"item": item, "price": price})
        print(f"Added {item} to menu for ${price}")
    
    def open_restaurant(self):
        self.is_open = True
        print(f"{self.name} is now OPEN!")

# Creating restaurants
pizza_place = Restaurant("Mario's Pizza", "Italian", 4.5)
# Output: Restaurant 'Mario's Pizza' established!

sushi_bar = Restaurant("Tokyo Sushi", "Japanese")
# Output: Restaurant 'Tokyo Sushi' established!

# Using the objects
pizza_place.add_menu_item("Margherita Pizza", 12.99)
pizza_place.open_restaurant()
```

### Destructor (`__del__`)

**Purpose**: Automatically called when an object is about to be destroyed or deleted.

#### Key Points:
- ✅ **Called automatically** during object deletion
- ✅ **Called only once** per object
- ✅ **Used for cleanup operations**

#### Real-World Example - File Manager:

```python
class FileManager:
    def __init__(self, filename):
        self.filename = filename
        self.file_handle = None
        print(f"FileManager created for '{filename}'")
    
    def open_file(self):
        print(f"Opening file: {self.filename}")
        self.file_handle = f"Handle for {self.filename}"
    
    def close_file(self):
        if self.file_handle:
            print(f"Closing file: {self.filename}")
            self.file_handle = None
    
    def __del__(self):
        # Cleanup when object is destroyed
        if self.file_handle:
            self.close_file()
        print(f"FileManager for '{self.filename}' destroyed!")

# Usage
file_mgr = FileManager("data.txt")
# Output: FileManager created for 'data.txt'

file_mgr.open_file()
# Output: Opening file: data.txt

del file_mgr
# Output: Closing file: data.txt
# Output: FileManager for 'data.txt' destroyed!
```

---

## Comprehensive Real-World Example

Let's create a complete example of a **Library Management System**:

```python
class Library:
    # Static variables (shared by all library objects)
    total_libraries = 0
    library_system = "City Library Network"
    
    def __init__(self, name, location):
        # Instance variables (unique for each library)
        self.name = name
        self.location = location
        self.books = []
        self.members = []
        self.is_open = False
        
        # Update static variable
        Library.total_libraries += 1
        print(f"Library '{self.name}' established at {self.location}")
    
    # Instance method
    def add_book(self, title, author, isbn):
        book = {
            "title": title,
            "author": author,
            "isbn": isbn,
            "is_available": True
        }
        self.books.append(book)
        print(f"Book '{title}' by {author} added to {self.name}")
    
    # Instance method
    def register_member(self, member_name, member_id):
        member = {
            "name": member_name,
            "id": member_id,
            "borrowed_books": []
        }
        self.members.append(member)
        print(f"Member '{member_name}' registered at {self.name}")
    
    # Instance method
    def open_library(self):
        self.is_open = True
        print(f"{self.name} is now OPEN for public!")
    
    # Class method
    @classmethod
    def get_total_libraries(cls):
        return f"Total libraries in {cls.library_system}: {cls.total_libraries}"
    
    # Class method
    @classmethod
    def change_system_name(cls, new_name):
        cls.library_system = new_name
        print(f"Library system renamed to: {new_name}")
    
    # Static method
    @staticmethod
    def calculate_fine(days_overdue):
        fine_per_day = 2  # $2 per day
        return days_overdue * fine_per_day
    
    # Static method
    @staticmethod
    def is_valid_isbn(isbn):
        return len(isbn) == 13 and isbn.isdigit()
    
    def __del__(self):
        Library.total_libraries -= 1
        print(f"Library '{self.name}' has been closed permanently")

# Creating library objects
central_library = Library("Central Library", "Downtown")
# Output: Library 'Central Library' established at Downtown

branch_library = Library("Branch Library", "Suburbs")
# Output: Library 'Branch Library' established at Suburbs

# Using instance methods
central_library.add_book("Python Programming", "John Smith", "1234567890123")
central_library.register_member("Alice Johnson", "M001")
central_library.open_library()

# Using class methods
print(Library.get_total_libraries())
# Output: Total libraries in City Library Network: 2

Library.change_system_name("Metropolitan Library System")
# Output: Library system renamed to: Metropolitan Library System

# Using static methods
fine = Library.calculate_fine(5)
print(f"Fine for 5 days overdue: ${fine}")  # Fine for 5 days overdue: $10

is_valid = Library.is_valid_isbn("1234567890123")
print(f"ISBN valid: {is_valid}")  # ISBN valid: True

# Demonstrating object destruction
del central_library
# Output: Library 'Central Library' has been closed permanently
```

---

## Summary

### Key Concepts Recap:

1. **Class**: Blueprint for creating objects
2. **Object**: Instance of a class with properties and behaviors
3. **Instance Variables**: Unique to each object
4. **Static Variables**: Shared by all objects of a class
5. **Local Variables**: Temporary variables in methods
6. **Instance Methods**: Bound to objects, use `self`
7. **Class Methods**: Bound to class, use `@classmethod` and `cls`
8. **Static Methods**: Independent, use `@staticmethod`
9. **Constructor**: `__init__` method for object initialization
10. **Destructor**: `__del__` method for cleanup
