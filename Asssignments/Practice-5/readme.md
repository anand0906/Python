### **1. Arithmetic Operators**  
#### **Problem Statement:**  
You are given two numbers. Perform all arithmetic operations (addition, subtraction, multiplication, division, floor division, modulus, and exponentiation) and return them in a **list** in the given order.  

#### **Sample Test Cases:**  
##### **Test Case 1:**  
**Input:**  
```
a = 10  
b = 3  
```  
**Output:**  
```
[13, 7, 30, 3.3333333333333335, 3, 1, 1000]  
```  
**Explanation:**  
- `10 + 3 = 13`  
- `10 - 3 = 7`  
- `10 * 3 = 30`  
- `10 / 3 = 3.3333...`  
- `10 // 3 = 3`  
- `10 % 3 = 1`  
- `10 ** 3 = 1000`  

---

### **2. Comparison Operators**  
#### **Problem Statement:**  
You are given two numbers. Return a **list** containing the results of all comparison operations (`==`, `!=`, `>`, `<`, `>=`, `<=`) applied to them in this order.  

#### **Sample Test Cases:**  
##### **Test Case 1:**  
**Input:**  
```
x = 7  
y = 10  
```  
**Output:**  
```
[False, True, False, True, False, True]  
```  
**Explanation:**  
- `7 == 10 → False`  
- `7 != 10 → True`  
- `7 > 10 → False`  
- `7 < 10 → True`  
- `7 >= 10 → False`  
- `7 <= 10 → True`  

---

### **3. Logical Operators**  
#### **Problem Statement:**  
You are given two boolean values. Return a **list** containing results of logical operations (`and`, `or`, `not`) in the following order:  
1. `a and b`  
2. `a or b`  
3. `not a`  
4. `not b`  

#### **Sample Test Cases:**  
##### **Test Case 1:**  
**Input:**  
```
a = True  
b = False  
```  
**Output:**  
```
[False, True, False, True]  
```  
**Explanation:**  
- `True and False → False`  
- `True or False → True`  
- `not True → False`  
- `not False → True`  

---

### **4. Identity Operators**  
#### **Problem Statement:**  
You are given two variables. Check whether they refer to the same object in memory using `is` and `is not` and return a **list**.  

#### **Sample Test Cases:**  
##### **Test Case 1:**  
**Input:**  
```
a = [1, 2, 3]  
b = [1, 2, 3]  
```  
**Output:**  
```
[False, True]  
```  
**Explanation:**  
- `a is b → False` (Different objects in memory, though values are the same)  
- `a is not b → True`  

##### **Test Case 2:**  
**Input:**  
```
a = 42  
b = 42  
```  
**Output:**  
```
[True, False]  
```  
**Explanation:**  
- `a is b → True` (Small integers are cached, so they refer to the same memory)  
- `a is not b → False`  

---

### **5. Membership Operators**  
#### **Problem Statement:**  
You are given a string and a character. Return a **list** containing results of `in` and `not in` operators.  

#### **Sample Test Cases:**  
##### **Test Case 1:**  
**Input:**  
```
string = "python"  
char = "y"  
```  
**Output:**  
```
[True, False]  
```  
**Explanation:**  
- `"y" in "python" → True`  
- `"y" not in "python" → False`  

##### **Test Case 2:**  
**Input:**  
```
string = "hello"  
char = "z"  
```  
**Output:**  
```
[False, True]  
```  
**Explanation:**  
- `"z" in "hello" → False`  
- `"z" not in "hello" → True`  

---

### **6. Membership in a List**
#### **Problem Statement:**  
Given a list `L` and an element `x`, return a **list** containing:
1. Whether `x` exists in `L`.
2. Whether `x` does not exist in `L`.

#### **Sample Test Cases:**  
##### **Test Case 1:**  
**Input:**  
```
L = ["apple", "banana", "cherry"]  
x = "banana"  
```  
**Output:**  
```
[True, False]  
```  
**Explanation:**  
- `'banana' in L → True`  
- `'banana' not in L → False`  

##### **Test Case 2:**  
**Input:**  
```
L = [1, 2, 3, 4]  
x = 5  
```  
**Output:**  
```
[False, True]  
```  
**Explanation:**  
- `5 in L → False`  
- `5 not in L → True`  

---
### **7. Arithmetic Puzzle**
#### **Problem Statement:**  
You are given two numbers `a` and `b`. Perform the following operations in order and return them in a **list**:
1. Multiply `a` by the remainder of `b` when divided by `a`.
2. Divide the sum of `a` and `b` by their difference (absolute value).
3. Add the square of `a` to the cube of `b`.

#### **Sample Test Cases:**  
##### **Test Case 1:**  
**Input:**  
```
a = 5, b = 8
```
**Output:**  
```
[15, 2.6, 537]
```
**Explanation:**  
- `5 * (8 % 5) = 5 * 3 = 15`
- `(5 + 8) / |5 - 8| = 13 / 3 = 2.6`
- `5^2 + 8^3 = 25 + 512 = 537`

---

### **8. Complex Comparison**
#### **Problem Statement:**  
You are given three numbers `x`, `y`, and `z`. Return a **list** containing:
1. Whether `x` is strictly greater than both `y` and `z`.
2. Whether `y` is the median value of the three numbers.
3. Whether all numbers are distinct.

#### **Sample Test Cases:**  
##### **Test Case 1:**  
**Input:**  
```
x = 12, y = 8, z = 15
```
**Output:**  
```
[False, True, True]
```
**Explanation:**  
- `12 > 8 and 12 > 15 → False`
- `8 is the median of (8, 12, 15) → True`
- `12, 8, 15 are distinct → True`

---

### **9. Logical Operations Challenge**
#### **Problem Statement:**  
Given three boolean values `A`, `B`, and `C`, return a **list** containing:
1. `(A and not B) or C`
2. `not (A or B) and C`
3. `A xor B xor C`

#### **Sample Test Cases:**  
##### **Test Case 1:**  
**Input:**  
```
A = True, B = False, C = True
```
**Output:**  
```
[True, False, False]
```
**Explanation:**  
- `(True and not False) or True → True`
- `not (True or False) and True → False`
- `True xor False xor True → False`

---

### **10. Identity and Membership Check**
#### **Problem Statement:**  
You are given a list `L` and an element `x`. Return a **list** containing:
1. Whether `x` is present in `L` and is the largest element.
2. Whether `x` is not in `L` but greater than all its elements.
3. Whether `L` contains at least one duplicate element.

#### **Sample Test Cases:**  
##### **Test Case 1:**  
**Input:**  
```
L = [3, 7, 2, 7]
x = 7
```
**Output:**  
```
[True, False, True]
```
**Explanation:**  
- `7 is in [3, 7, 2, 7] and 7 is the max → True`
- `7 is in L, so cannot be greater than all its elements → False`
- `7 appears twice in L → True`

---

### **11. Advanced Membership Testing**
#### **Problem Statement:**  
You are given a string `S` and a substring `sub`. Return a **list** containing:
1. Whether `sub` is present in `S`.
2. Whether reversing `sub` is present in `S`.
3. Whether `S` starts and ends with `sub`.

#### **Sample Test Cases:**  
##### **Test Case 1:**  
**Input:**  
```
S = "racecar"
sub = "car"
```
**Output:**  
```
[True, False, False]
```
**Explanation:**  
- `'car' in "racecar" → True`
- `'rac' (reverse of 'car') in "racecar" → False`
- `"racecar" does not start and end with 'car' → False`

---



