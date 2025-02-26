<details>
<summary>1. Name Tag Formatter</summary>

```python
name=input()
temp=name.lower()
ans=temp.title()
print(ans)
```
</details>

---

<details>
<summary>2.  Document Title Formatter</summary>

```python
doc_title=input()
print(doc_title.capitalize())
```
</details>

---

<details>
<summary>3. Secret Code Generator</summary>

```python
message=input()
print(message.swapcase())
```
</details>

---
<details>
<summary>4. Loudspeaker Announcement </summary>

```python
announce=input()
print(announce.upper())
```
</details>

---
<details>
<summary>5. Whisper Mode</summary>

```python
message=input()
print(message.lower())
```
</details>

---
<details>
<summary>6. Censorship System</summary>

```python
s=input()
print(s.replace("bad","***"))
```
</details>

---
<details>
<summary>7. Auto-Correct System</summary>

```python
message=input()
message=message.replace("r ","are ")
message=message.replace("u ","you ")
print(message)
```
</details>

---
<details>
<summary>8. Space Trimmer</summary>

```python
email=input()
print(email.strip())
```
</details>

---
<details>
<summary>9. Check If Input Is Numeric</summary>

```python
amount=input()
print(amount.isnumeric())
```
</details>

---
<details>
<summary>10.  Check If Input Contains Only Alphabets</summary>

```python
name=input()
print(name.isalpha())
```
</details>

---

<details>
<summary>11. String Formatting: Dynamic Greeting Message</summary>

```python
name=input()
print("Hello, {}! Welcome to our platform.".format(name))
```
</details>

---

<details>
<summary>11. String Formatting: Report Card Generator</summary>

```python
name=input()
percentage=float(input())
print("Student: {} | Score: {:.2f}%".format(name,percentage))
```
</details>

---

<details>
<summary>12. String Formatting: Product Price Tag</summary>

```python
name=input()
price=float(input())
print("Product: {} | Score: {:.2f}".format(name,price))
```
</details>
