## Problem 1: Library Book Management

**Problem Description:**
Design a `Book` class to manage book details.

* Instance Variables: `title`, `author`, `price`
* Class Variable: `total_books`
* Methods: display book details, show total number of books

**Rough Blueprint:**

```
Class: Book
 ├── Instance Variables: title, author, price
 ├── Class Variable: total_books
 ├── Constructor(title, author, price)
 ├── Method: display_book()
 ├── Class Method: show_total_books()
```

**Sample Test Cases:**

```
# Test Case 1
Input:
b1 = Book("Rich Dad Poor Dad", "Robert Kiyosaki", 450)
b1.display_book()
Book.show_total_books()

Output:
Title: Rich Dad Poor Dad, Author: Robert Kiyosaki, Price: 450
Total Books: 1

# Test Case 2
Input:
b2 = Book("Atomic Habits", "James Clear", 550)
b2.display_book()
Book.show_total_books()

Output:
Title: Atomic Habits, Author: James Clear, Price: 550
Total Books: 2
```

---

## Problem 2: Bank Account System

**Problem Description:**
Create a `BankAccount` class.

* Instance Variables: `account_number`, `holder_name`, `balance`
* Constant (final variable): `IFSC_CODE`
* Methods: deposit, withdraw, display balance

**Rough Blueprint:**

```
Class: BankAccount
 ├── Instance Variables: account_number, holder_name, balance
 ├── Constant: IFSC_CODE = "SBIN0001234"
 ├── Constructor(account_number, holder_name, balance)
 ├── Method: deposit(amount)
 ├── Method: withdraw(amount)
 ├── Method: display_balance()
```

**Sample Test Cases:**

```
# Test Case 1
Input:
acc1 = BankAccount("12345", "Anand", 1000)
acc1.deposit(500)
acc1.display_balance()

Output:
Deposited: 500
Balance: 1500

# Test Case 2
Input:
acc1.withdraw(200)
acc1.display_balance()

Output:
Withdrawn: 200
Balance: 1300

# Test Case 3 (Edge Case - insufficient funds)
Input:
acc1.withdraw(2000)

Output:
Insufficient Balance
```

---

## Problem 3: Student Grade Calculator

**Problem Description:**
Create a `Student` class.

* Instance Variables: `name`, `marks[]`
* Class Variable: `total_students`
* Methods: calculate average, get grade

**Rough Blueprint:**

```
Class: Student
 ├── Instance Variables: name, marks[]
 ├── Class Variable: total_students
 ├── Constructor(name, marks[])
 ├── Method: calculate_average() → float
 ├── Method: get_grade() → char
```

**Sample Test Cases:**

```
# Test Case 1
Input:
s1 = Student("Ravi", [80, 70, 90])
print(s1.calculate_average())
print(s1.get_grade())

Output:
80.0
B

# Test Case 2
Input:
s2 = Student("Meena", [95, 92, 90])
print(s2.calculate_average())
print(s2.get_grade())

Output:
92.33
A

# Test Case 3 (Edge Case - low marks)
Input:
s3 = Student("Arun", [40, 35, 30])
print(s3.calculate_average())
print(s3.get_grade())

Output:
35.0
F
```

---

## Problem 4: Employee Salary Management

**Problem Description:**
Create an `Employee` class.

* Instance Variables: `emp_id`, `name`, `basic_salary`
* Class Variable: `company_name`
* Methods: set/get salary, calculate net salary after tax (10%)

**Rough Blueprint:**

```
Class: Employee
 ├── Instance Variables: emp_id, name, basic_salary
 ├── Class Variable: company_name = "Infosys"
 ├── Constructor(emp_id, name, basic_salary)
 ├── Method: set_salary(salary)
 ├── Method: get_salary()
 ├── Method: calculate_net_salary() → float
```

**Sample Test Cases:**

```
# Test Case 1
Input:
e1 = Employee(101, "Anand", 50000)
print(e1.calculate_net_salary())

Output:
45000.0

# Test Case 2
Input:
e1.set_salary(60000)
print(e1.get_salary())
print(e1.calculate_net_salary())

Output:
60000
54000.0

# Test Case 3 (Different Employee)
Input:
e2 = Employee(102, "Ravi", 40000)
print(e2.calculate_net_salary())

Output:
36000.0
```

---

## Problem 5: Shopping Cart

**Problem Description:**
Create a `Product` class.

* Instance Variables: `name`, `price`, `quantity`
* Class Variable: `total_bill`
* Methods: calculate total price for product, update total bill
* Local Variable: temporary calculation inside method

**Rough Blueprint:**

```
Class: Product
 ├── Instance Variables: name, price, quantity
 ├── Class Variable: total_bill
 ├── Constructor(name, price, quantity)
 ├── Method: calculate_total()
     └── Local Variable: item_total = price * quantity
```

**Sample Test Cases:**

```
# Test Case 1
Input:
p1 = Product("Laptop", 40000, 1)
print(p1.calculate_total())

Output:
Item Total (Laptop): 40000

# Test Case 2
Input:
p2 = Product("Mouse", 500, 2)
print(p2.calculate_total())

Output:
Item Total (Mouse): 1000

# Test Case 3
Input:
print("Total Bill:", Product.total_bill)

Output:
Total Bill: 41000

# Test Case 4 (Adding more products)
Input:
p3 = Product("Keyboard", 1500, 1)
print(p3.calculate_total())
print("Total Bill:", Product.total_bill)

Output:
Item Total (Keyboard): 1500
Total Bill: 42500
```

---
