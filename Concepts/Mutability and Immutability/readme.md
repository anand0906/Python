# **Mutability vs. Immutability in Python**

## **🔹 What is Mutability?**  
📌 **Mutability** is a property that states that **the internal state (value) of an object can be modified after its creation.**  
➡️ Simply, we can **make changes to an object** without creating a new one.  

✅ **Examples of Mutable Objects:**  
- **List** (`list`)  
- **Set** (`set`)  
- **Dictionary** (`dict`)  

🟢 **Changing value is cheap** (modifications happen in place).  

### **🔹 Example: Mutable List**
```python
fruits = ["Apple", "Banana", "Cherry"]
print(id(fruits))  # Print memory address before modification
fruits.append("Mango")  # Adding an item
print(fruits)  # Output: ['Apple', 'Banana', 'Cherry', 'Mango']
print(id(fruits))  # Memory address remains the same
```
✅ The original **list is modified** instead of creating a new list.  

---

## **🔹 What is Immutability?**  
📌 **Immutability** is a property that states that **the internal state of an object can't be modified after its creation.**  
➡️ Simply, we **cannot make changes** to an object directly.  
➡️ If we need to modify it, **a new object must be created** instead of altering the existing one.  

🚫 **Examples of Immutable Objects:**  
- **Integer** (`int`)  
- **Float** (`float`)  
- **String** (`str`)  
- **Tuple** (`tuple`)  
- **Frozen Set** (`frozenset`)  

🔴 **Changing values is expensive** (since new objects are created).  

### **🔹 Example: Immutable String**
```python
name = "Anand"
print(id(name))  # Print memory address before modification
name = name + " Pasam"  # Creates a new string
print(name)  # Output: 'Anand Pasam'
print(id(name))  # Memory address changes
```
🚫 The original **string is not modified**, a new string is created instead.

✅ **Correct way (creating a new object)**  
```python
name = "Anand"
new_name = "B" + name[1:]  # Creates a new string
print(new_name)  # Output: 'Bnand'
```
📌 A **new string is created**, and the original one remains unchanged.

---

## **🔹 Key Differences: Mutable vs Immutable**
| Feature | Mutable Objects (Lists, Dicts, Sets) | Immutable Objects (Tuples, Strings, Ints) |
|---------|---------------------------------|----------------------------------|
| Can be changed? | ✅ Yes | ❌ No |
| Memory Address  | 🔄 Same after modification | 🔄 New object created |
| Performance    | 🚀 Faster for frequent modifications | 🚀 Safer and more efficient for fixed values |
| Example  | `list = [1, 2, 3]`  | `tuple = (1, 2, 3)` |

---
