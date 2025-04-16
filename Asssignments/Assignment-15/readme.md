## 🧱 1. Easy Patterns

---

### **Pattern 1: Stars in a Single Row**

#### 📝 Problem Statement:
Print a single row of `n` stars.

#### ✅ Sample Input:
```
n = 5
```

#### 🔍 Output:
```
* * * * *
```

#### 📘 Explanation:
Print `*` `n` times with a space in between.

---

### **Pattern 2: Increasing Numbers in a Row**

#### 📝 Problem Statement:
Print numbers from `1` to `n` in a single row.

#### ✅ Sample Input:
```
n = 5
```

#### 🔍 Output:
```
1 2 3 4 5
```

#### 📘 Explanation:
Loop from `1` to `n`, print each number.

---

### 🔁 Reverse Format:
#### 🔁 Output:
```
5 4 3 2 1
```

---

### **Pattern 3: Alphabets in Single Row**

#### 📝 Problem Statement:
Print capital alphabets from `A` to corresponding letter for `n`.

#### ✅ Sample Input:
```
n = 5
```

#### 🔍 Output:
```
A B C D E
```

#### 📘 Explanation:
Loop from `0` to `n-1`, use `chr(65 + i)` to print alphabet letters.

---

### 🔁 Reverse Format:
#### 🔁 Output:
```
E D C B A
```

---

## 🔲 2. Medium Patterns

---

### **Pattern 4: Square of Stars**

#### 📝 Problem Statement:
Print an `n x n` square of stars.

#### ✅ Sample Input:
```
n = 3
```

#### 🔍 Output:
```
* * *
* * *
* * *
```

#### 📘 Explanation:
Outer loop: rows → 3  
Inner loop: columns → 3 stars per row

---

### 🔁 Reverse Format:
#### 🔁 Output:
```
* * *
* * *
* * *
```
(Same since all rows are identical)

---

### **Pattern 5: Increasing Numbers Row-wise**

#### 📝 Problem Statement:
Print rows where each row has numbers from 1 to `n`.

#### ✅ Sample Input:
```
n = 4
```

#### 🔍 Output:
```
1 2 3 4
1 2 3 4
1 2 3 4
1 2 3 4
```

---

### 🔁 Reverse Format:
#### 🔁 Output:
```
4 3 2 1
4 3 2 1
4 3 2 1
4 3 2 1
```

---

### **Pattern 6: Right-Angled Star Triangle**

#### 📝 Problem Statement:
Print a right-angled triangle with stars increasing row by row.

#### ✅ Sample Input:
```
n = 4
```

#### 🔍 Output:
```
*
* *
* * *
* * * *
```

#### 📘 Explanation:
Row `i` has `i` stars.

---

### 🔁 Reverse Format:
#### 🔁 Output:
```
* * * *
* * *
* *
*
```

---

### **Pattern 7: Number Triangle (1 to n per row)**

#### 📝 Problem Statement:
Print a triangle where each row contains numbers from `1` to the row number.

#### ✅ Sample Input:
```
n = 4
```

#### 🔍 Output:
```
1
1 2
1 2 3
1 2 3 4
```

---

### 🔁 Reverse Format:
#### 🔁 Output:
```
1 2 3 4
1 2 3
1 2
1
```

---

## 🔺 3. Harder Patterns

---

### **Pattern 8: Alphabet Triangle**

#### 📝 Problem Statement:
Print a triangle where each row has alphabets from `A` up to the corresponding row length.

#### ✅ Sample Input:
```
n = 4
```

#### 🔍 Output:
```
A
A B
A B C
A B C D
```

---

### 🔁 Reverse Format:
#### 🔁 Output:
```
A B C D
A B C
A B
A
```

---

### **Pattern 9: Repeating Alphabets in Triangle**

#### 📝 Problem Statement:
Each row prints the same letter, repeating `row number` times starting from A.

#### ✅ Sample Input:
```
n = 4
```

#### 🔍 Output:
```
A
B B
C C C
D D D D
```

---

### 🔁 Reverse Format:
#### 🔁 Output:
```
D D D D
C C C
B B
A
```

