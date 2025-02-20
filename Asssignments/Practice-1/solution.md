<details>
<summary>1. Calculate the Year When the User Turns 100</summary>

```python
name = input("Enter your name: ")
age = int(input("Enter your age: "))
remainingYears = 100 - age
ans = 2025 + remainingYears
print(name, "will turn 100 in", ans)
```

**Steps:**
1. Take the user's name as input.
2. Take the user's age as input.
3. Calculate the remaining years to reach 100.
4. Add those years to the current year (2025).
5. Print the year in which the user will turn 100.

</details>

---

<details>
<summary>2. Swap Two Numbers Using Arithmetic Operations</summary>

```python
num1 = int(input())
num2 = int(input())
num1 = num1 + num2
num2 = num1 - num2
num1 = num1 - num2
print(num1, num2)
```

**Steps:**
1. Take two numbers as input.
2. Add both numbers and store the result in `num1`.
3. Subtract `num2` from the new `num1` to get the original `num1` value in `num2`.
4. Subtract the new `num2` from `num1` to get the original `num2` value in `num1`.
5. Print the swapped numbers.

</details>

---

<details>
<summary>3. Perform All Arithmetic Operations</summary>

```python
num1 = int(input())
num2 = int(input())
print("Addition:", num1 + num2)
print("Subtraction:", num1 - num2)
print("Multiplication:", num1 * num2)
print("Division:", num1 // num2)
print("Modulus:", num1 % num2)
```

**Steps:**
1. Take two numbers as input.
2. Perform addition, subtraction, multiplication, integer division, and modulus operations.
3. Print the results.

</details>

---

<details>
<summary>4. Calculate Area and Perimeter of a Rectangle</summary>

```python
length = int(input())
width = int(input())
area = length * width
perimeter = 2 * (length + width)
print("Area:", area)
print("Perimeter:", perimeter)
```

**Steps:**
1. Take length and width as input.
2. Calculate the area using `length * width`.
3. Calculate the perimeter using `2 * (length + width)`.
4. Print the area and perimeter.

</details>

---

<details>
<summary>5. Convert Celsius to Fahrenheit</summary>

```python
celsius = float(input())
fahrenheit = (9/5) * celsius + 32
print(fahrenheit)
```

**Steps:**
1. Take the temperature in Celsius as input.
2. Convert it to Fahrenheit using the formula `(9/5) * Celsius + 32`.
3. Print the Fahrenheit temperature.

</details>

---

<details>
<summary>6. Calculate Simple Interest</summary>

```python
p = int(input())
r = int(input())
t = int(input())
simpleInterest = (p * r * t) / 100
print(simpleInterest)
```

**Steps:**
1. Take principal (`p`), rate of interest (`r`), and time (`t`) as input.
2. Calculate simple interest using the formula `(P * R * T) / 100`.
3. Print the simple interest.

</details>

---

<details>
<summary>7. Find Sum of Digits of a 3-Digit Number</summary>

```python
num = int(input())
ones = num % 10
num = num // 10
tens = num % 10
num = num // 10
hundreds = num % 10
print(ones + tens + hundreds)
```

**Steps:**
1. Take a 3-digit number as input.
2. Extract the ones place digit using `num % 10`.
3. Remove the ones place digit using integer division `num // 10`.
4. Extract the tens place digit and repeat the process for the hundreds place.
5. Add all three digits and print the sum.

</details>

---

<details>
<summary>8. Reverse a 3-Digit Number</summary>

```python
num = int(input())
ones = num % 10
num = num // 10
tens = num % 10
num = num // 10
hundreds = num % 10
print(ones * 100 + tens * 10 + hundreds)
```

**Steps:**
1. Take a 3-digit number as input.
2. Extract each digit (ones, tens, hundreds) using modulus and division.
3. Reconstruct the number in reverse order.
4. Print the reversed number.

</details>

---

<details>
<summary>9. Convert Total Minutes to Hours and Minutes</summary>

```python
minutes = int(input())
hour = minutes // 60
minute = minutes % 60
print(hour, ":", minute, sep="")
```

**Steps:**
1. Take the total minutes as input.
2. Convert to hours by performing integer division `minutes // 60`.
3. Get the remaining minutes using `minutes % 60`.
4. Print the result in `hours:minutes` format.

</details>

---

<details>
<summary>10. Sum of First N Natural Numbers</summary>

```python
n = int(input())
sum = n * (n + 1) // 2
print(sum)
```

**Steps:**
1. Take a number `N` as input.
2. Use the formula `N * (N + 1) / 2` to find the sum.
3. Print the result.

</details>

---

<details>
<summary>11. Find Square and Cube of a Number</summary>

```python
n = int(input())
print("Square:", n**2)
print("Cube:", n**3)
```

**Steps:**
1. Take a number as input.
2. Calculate the square using `n**2`.
3. Calculate the cube using `n**3`.
4. Print both results.

</details>
