## **List**
------
A list is a built-in data type (or) data structure in Python, which represents a collection of data items and has the following features:

1. **Mutable (or) changeable**
2. **Ordered**
3. **Allows duplicates**
4. **Can store any type of data**
5. **Can be of any length**

### **Examples:**
```python
list1 = [1, 3, 4]
list2 = [1, "anand"]
list3 = [[1, 2, 3], "abc", 3]
```

---

## **Operations on List:**
1. **Creating a list**
2. **Adding elements to a list**
3. **Accessing elements in a list**
4. **Updating elements in a list**
5. **Deleting elements from a list**

---

## **3. Accessing Elements of a List**

| **List Indexing**      | **List Slicing**      |
|----------------------|---------------------|
| `a = [1,2,3,"abc"]` | `a = [10,20,30,40]` |
| `a[0]` → `1`        | `a[1:3]` → `[20,30]` |
| `a[3]` → `"abc"`    | `a[0:3]` → `[10,20,30]` |
| `a[-1]` → `"abc"`   | `a[:2]` → `[10,20]` |
| `a[10]` → `IndexError` | `a[3:]` → `[40]` |
| `a[-22]` → `IndexError` | `a[10:20]` → `[]` |
|                      | `a[0:3:2]` → `[10,30]` |

---

## **4. Updating Elements of a List**
🔹 We can update a **single element** using list indexing.
🔹 We can update **multiple elements** using list slicing.

### **Updating Single Elements:**
```python
a = [1,2,3]
a[2] = 5
print(a)  # Output: [1,2,5]
```
```python
a = ["a","b"]
a[0] = [1,2,3]
print(a)  # Output: [[1,2,3],"b"]
```
```python
a = [1,2,3]
a[2] = "and"
print(a)  # Output: [1,2,"and"]
```

### **Updating Multiple Elements:**
🔹 The step size should always be equal to **one** when updating multiple elements.
```python
a = [1,2,3,4]
a[1:3] = [5,6]
print(a)  # Output: [1,5,6,4]
```
```python
a = [1,3,4,5,5]
a[1:4] = [1,2,3,4,5,6]
print(a)  # Output: [1,1,2,3,4,5,6,5]
```

---

## **5. Deleting Elements of a List**

### **Methods for Deletion:**
1. `remove()`
2. `pop()`
3. `clear()`
4. `del`

### **remove()**
🔹 Used to remove a specific **existing** element from the list.
🔹 If the element does not exist, it raises a `ValueError`.
🔹 Removes only **one occurrence** at a time.
🔹 **Return type:** `None`

```python
a = [1,3,4]
a.remove(3)
print(a)  # Output: [1,4]
```
```python
a = [1,2,3,4,4]
a.remove(4)
print(a)  # Output: [1,2,3,4]
```
🚫 **Error Case:**
```python
a = [1,3]
a.remove(5)  # ValueError: list.remove(x): x not in list
```

---

### **pop()**
🔹 Removes an element by its **index** and returns it.
🔹 **Return type:** value

```python
a = [1,2,3,4]
a.pop()
print(a)  # Output: [1,2,3]
```
```python
q = [1,2,3]
q.pop(0)
print(q)  # Output: [2,3]
```
```python
a = [1,2,3,5,6]
b = a.pop(4)
print(b)  # Output: 6
print(a)  # Output: [1,2,3,5]
```

---

### **del**
🔹 A keyword used to delete elements by index or the entire list.

```python
a = [1,3,4]
del a[2]
print(a)  # Output: [1,3]
```
```python
a = [1,2]
del a[0]
print(a)  # Output: [2]
```
🚫 **Error Case:**
```python
a = [1,2,3]
del a[10]  # IndexError
```

---

### **clear()**
🔹 Removes **all elements** from the list.
🔹 **Return type:** `None`

```python
a = [1,3,4,5]
a.clear()
print(a)  # Output: []
```
```python
a = ["ana","bcd"]
a.clear()
print(a)  # Output: []
```
---
## **Other Methods in List**

### **count()**
🔹 Returns the number of times a given value appears in the list.
🔹 **Return type:** `int`

**Example:**
```python
a = [1,3,4,5,3]
c = a.count(3)
print(c)  # Output: 2
```
```python
a = ["ab",3,4,"ab","ab"]
c = a.count("ab")
print(c)  # Output: 3
```

---

### **index()**
🔹 Finds the position (index) of a given value in the list.
🔹 **Return type:** `int`

**Example:**
```python
a = [1,2,3,4]
i = a.index(2)
print(i)  # Output: 1
```
```python
a = [1,"a","c",2]
ind = a.index(4)  # ValueError if element not found
print(ind)
```

#### **Special Case: index(value, start, end)**
```python
a = [1,3,4,4,5,4,4]
ind = a.index(4,4,6)
print(ind)  # Output: 5
```
```python
a = [1,2,3,3,3,3,3,5]
ind = a.index(3,-4,-1)
print(ind)  # Output: 4
```

---

### **reverse()**
🔹 Reverses the given list.
🔹 **Return type:** `None`

**Example:**
```python
a = [1,2,3,4]
a.reverse()
print(a)  # Output: [4,3,2,1]
```
```python
a = ["a","b","c"]
a.reverse()
print(a)  # Output: ["c","b","a"]
```

---

### **sort()**
🔹 Sorts the list in ascending or descending order.
🔹 **Note:** Every element in the list must be of the same type (comparable).

#### **Ascending Order (Default)**
```python
a = [3,2,10]
a.sort()
print(a)  # Output: [2,3,10]
```
```python
a = ["x","b","d"]
a.sort()
print(a)  # Output: ["b","d","x"]
```
```python
a = [[1],[4],[0]]
a.sort()
print(a)  # Output: [[0],[1],[4]]
```

#### **Descending Order**
```python
a = [3,2,10]
a.sort(reverse=True)
print(a)  # Output: [10,3,2]
```
```python
a = ["x","b","d"]
a.sort(reverse=True)
print(a)  # Output: ["x","d","b"]
```

---

## **Special Methods in List**

| Method  | Description |
|---------|-------------|
| `len()` | Returns the length of the list |
| `max()` | Returns the maximum element of the list |
| `min()` | Returns the minimum element of the list |
| `sorted()` | Returns a sorted copy of the list |

**Example:**
```python
a = [1,2,3]
length = len(a)
print(length)  # Output: 3
```
```python
a = [2,3,4]
s = max(a)
print(s)  # Output: 4
```
```python
a = [1,2,4]
s = min(a)
print(s)  # Output: 1
```

#### **Using `sorted()`**
```python
a = [2,1,3]
temp = sorted(a)
temp_r = sorted(a, reverse=True)
print(temp)   # Output: [1,2,3]
print(temp_r) # Output: [3,2,1]
```



