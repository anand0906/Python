<details>
<summary>1. Calculate the Year When the User Turns 100</summary>
  
```python
name=input("Enter you name :")
age=int(input("Enter your age :"))
remainingYears=100-age
ans=2025+remainingYears
print(name,"will turn 100 in",ans)
```
</details>

---

<details>
<summary>2. Swap Two Numbers Using Arithmetic Operations</summary>
  
```python
num1=int(input())
num2=int(input())
num1=num1+num2
num2=num1-num2
num1=num1-num2
print(num1,num2)
```
</details>

---

<details>
<summary>3. Perform All Arithmetic Operations</summary>
  
```python
num1=int(input())
num2=int(input())
print("Addition:",num1+num2)
print("Subtraction:",num1-num2)
print("Multiplication:",num1*num2)
print("Division:",num1//num2)
print("Modulus:",num1%num2)
```
</details>

---

<details>
<summary>4. Calculate area and Perimeter of a Rectangle</summary>
  
```python
length=int(input())
width=int(input())
area=length*width
perimeter=2*(length+width)
print("Area:",area)
print("Perimeter:",perimeter)
```
</details>

---

<details>
<summary>5. Convert Celsius to Fahrenheit</summary>
  
```python
celsius=float(input())
fahrenheit=(9/5)*celsius+32
print(fahrenheit)
```
</details>

---

<details>
<summary>6. Calculate Simple Interest</summary>
  
```python
p=int(input())
r=int(input())
t=int(input())
simpleIntrest=(p*r*t)/100
print(simpleIntrest)
```
</details>

---

<details>
<summary>7. Find Sum of Digits of a 3-Digit Number</summary>
  
```python
num=int(input())
ones=num%10
num=num//10
tens=(num%10)
num=num//10
hundreds=(num%10)
print(ones+tens+hundreds)
```
</details>

---

<details>
<summary>Reverse a 3-Digit Number</summary>
  
```python
num=int(input())
ones=num%10
num=num//10
tens=(num%10)
num=num//10
hundreds=(num%10)
print(ones*100+tens*10+hundreds*1)
```
</details>

---

<details>
<summary>Convert Total Minutes to Hours and Minutes</summary>
  
```python
minutes=int(input())
hour=minutes//60
minute=minutes%60
print(hour,":",minute,sep="")
```
</details>

---

<details>
<summary>10. Sum of First N Natural Numbers</summary>
  
```python
n=int(input())
sum=n*(n+1)//2
print(sum)
```
</details>

---

<details>
<summary>11. Find Square and Cube of a Number</summary>
  
```python
n=int(input())
print("square:",n**2)
print("Cube:",n**3)
```
</details>


---
