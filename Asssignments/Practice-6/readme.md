### 1. Who Has More Followers?
#### Problem Statement:
You are given the follower counts of two social media influencers, `Alice` and `Bob`. Return a tuple where:
- First element: `Alice's followers > Bob's followers`
- Second element: `Alice's followers < Bob's followers`
- Third element: `Alice's followers == Bob's followers`

#### Sample Test Cases:
**Input:**  
```python
alice_followers = 5000  
bob_followers = 7000  
```
**Output:**  
```python
(False, True, False)
```
**Explanation:**  
- `5000 > 7000` → `False`  
- `5000 < 7000` → `True`  
- `5000 == 7000` → `False`  

---

### 2. VIP Club Membership Check
#### Problem Statement:
A club has an exclusive VIP list. You are given a name and must check if the person is in the VIP list.  
Return `True` if the person is in the list, otherwise return `False`.

#### Sample Test Cases:
**Input:**  
```python
vip_list = ["Elon", "Bill", "Steve", "Sundar"]  
person = "Sundar"  
```
**Output:**  
```python
True
```
**Explanation:**  
Since `"Sundar"` is in the `vip_list`, the result is `True`.

---

### 3. Battery Sufficient for a Trip?
#### Problem Statement:
A car’s battery percentage is given. Return `True` if the battery is **greater than or equal to 60%**, otherwise return `False`.

#### Sample Test Cases:
**Input:**  
```python
battery_percentage = 75  
```
**Output:**  
```python
True
```
**Explanation:**  
Since `75 >= 60`, the result is `True`.

---

### 4. Streaming Plan Upgrade Check
#### Problem Statement:
A user has a **basic** streaming subscription. If their usage is greater than **200 hours per month**, they need to upgrade.  
Return `True` if an upgrade is required, otherwise return `False`.

#### Sample Test Cases:
**Input:**  
```python
current_usage = 250  
```
**Output:**  
```python
True
```
**Explanation:**  
Since `250 > 200`, the result is `True`.

---

### 5. Social Media Friend Suggestion
#### Problem Statement:
A mutual friends list is given. Return `True` if a person is in the mutual friends list, otherwise return `False`.

#### Sample Test Cases:
**Input:**  
```python
mutual_friends = ["John", "Emma", "Sophia"]  
person = "Emma"  
```
**Output:**  
```python
True
```
**Explanation:**  
Since `"Emma"` is in `mutual_friends`, the result is `True`.

---

### 6. Logical AND: Are Both Apps Installed?
#### Problem Statement:
A user has a list of installed apps. Return `True` if both "WhatsApp" and "Instagram" are installed, otherwise return `False`.

#### Sample Test Cases:
**Input:**  
```python
installed_apps = ["WhatsApp", "Facebook", "Instagram"]  
```
**Output:**  
```python
True
```
**Explanation:**  
Both `"WhatsApp"` and `"Instagram"` are present, so the result is `True`.

---

### 7. Logical OR: Can Access Premium Content?
#### Problem Statement:
A user can access premium content if they either have a **"Premium"** subscription or **more than 5000 reward points**.  
Return `True` if they can access it, otherwise return `False`.

#### Sample Test Cases:
**Input:**  
```python
subscription = "Free"  
reward_points = 6000  
```
**Output:**  
```python
True
```
**Explanation:**  
Even though the subscription is "Free", the user has `6000 > 5000` reward points, so they can access premium content.

---

### 8. Logical NOT: Is the Device Not in the Blacklist?
#### Problem Statement:
A list of **blacklisted devices** is given. If a user’s device is NOT in the blacklist, return `True`, otherwise return `False`.

#### Sample Test Cases:
**Input:**  
```python
blacklisted_devices = ["iPhone 6", "Samsung J7", "Nokia 3310"]  
device = "iPhone 12"  
```
**Output:**  
```python
True
```
**Explanation:**  
Since `"iPhone 12"` is NOT in `blacklisted_devices`, the result is `True`.

---

### 9. Who Has the Newer Phone?
#### Problem Statement:
Two users have different phone models with release years. Return a tuple where:
- First element: `User A's phone is newer`
- Second element: `User B's phone is newer`
- Third element: `Both have the same phone`

#### Sample Test Cases:
**Input:**  
```python
user_a_phone = ("iPhone 12", 2020)  
user_b_phone = ("iPhone 14", 2022)  
```
**Output:**  
```python
(False, True, False)
```
**Explanation:**  
Since `2022 > 2020`, User B has the newer phone.

---

### 10. Does the Password Contain Special Characters?
#### Problem Statement:
A strong password must contain at least one special character (`!@#$%^&*`).  
Return `True` if the password contains a special character, otherwise return `False`.

#### Sample Test Cases:
**Input:**  
```python
password = "Pass@word123"  
```
**Output:**  
```python
True
```
**Explanation:**  
The password contains `@`, which is a special character.

