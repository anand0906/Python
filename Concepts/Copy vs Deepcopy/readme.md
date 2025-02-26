## **copy() and deepcopy()**

### **Types of Copying:**
1. **Shallow Copy**
2. **Deep Copy**

---

## **1. Shallow Copy**
🔹 Creates a **new list** and copies the **references** of all the values from the original list into the new list.
🔹 Changes in nested objects **reflect** in both lists because they share the same reference.
🔹 **Return type:** `list`

**Example:**
```python
temp = [1, 2, 3, 4, 5, 6]
c = temp.copy()
print(temp, c)
```
**Output:**
```python
[1, 2, 3, 4, 5, 6]  [1, 2, 3, 4, 5, 6]
```

### **Problem with Shallow Copy:**
🔹 If the original list contains nested lists, modifying the nested list in one copy **affects** the other copy.

**Example:**
```python
a = [1, 2, [1, 2, 3]]
b = a.copy()
print(a, b)

b[2].append(5)
print(a, b)
```
**Output:**
```python
[1, 2, [1, 2, 3]]  [1, 2, [1, 2, 3]]
[1, 2, [1, 2, 3, 5]]  [1, 2, [1, 2, 3, 5]]
```
📌 **Issue:** The change in `b[2]` reflects in `a[2]` because both lists share the same reference.

---

## **2. Deep Copy**
🔹 Recursively **creates a new list** along with **new copies** of nested objects.
🔹 Changes in the copied list **do not** affect the original list.

**Example:**
```python
import copy

a = [1, 3, [1, 2, 3]]
b = copy.deepcopy(a)
print(a, b)

b[2].append(5)
print(a, b)
```
**Output:**
```python
[1, 3, [1, 2, 3]]  [1, 3, [1, 2, 3]]
[1, 3, [1, 2, 3]]  [1, 3, [1, 2, 3, 5]]
```
📌 **Solution:** `deepcopy()` ensures that changes in `b` **do not** affect `a`, as each element is independently copied.

