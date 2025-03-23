### 1. Smart Home Mode Selection  
#### Problem:  
A smart home system offers three modes based on the time of day:
- **"Morning Mode"** → If the time is between 5:00 AM and 11:59 AM  
- **"Evening Mode"** → If the time is between 5:00 PM and 9:59 PM  
- **"Night Mode"** → If the time is between 10:00 PM and 4:59 AM  
- **"Day Mode"** → Any other time  

Take a **24-hour format time (HH:MM)** as input and determine the appropriate mode.  

#### Sample Test Cases:  
##### Test Case 1:  
**Input:**  
```
time = "06:30"
```  
**Output:**  
```
Morning Mode
```  
**Explanation:** The time is between 5:00 AM and 11:59 AM, so it is "Morning Mode".  

##### Test Case 2:  
**Input:**  
```
time = "22:15"
```  
**Output:**  
```
Night Mode
```  
**Explanation:** The time is between 10:00 PM and 4:59 AM, so it is "Night Mode".  

---

### 2. Virtual Assistant Response  
#### Problem:  
A virtual assistant responds differently based on the **type of request**:
- If the message **starts with "Hey" or "Hello"**, respond with "How can I help you?"  
- If the message **contains "weather"**, respond with "Fetching weather details..."  
- If the message **ends with a question mark "?"**, respond with "Let me find that for you."  
- Otherwise, respond with "I'm here if you need anything."  

#### Sample Test Cases:  
##### Test Case 1:  
**Input:**  
```
message = "Hey Assistant"
```  
**Output:**  
```
How can I help you?
```  
**Explanation:** The message starts with "Hey", so the assistant responds accordingly.  

##### Test Case 2:  
**Input:**  
```
message = "What's the weather today?"
```  
**Output:**  
```
Fetching weather details...
```  
**Explanation:** The message contains "weather", so the assistant provides weather details.  

---

### 3. Smart Notification Filter  
#### Problem:  
A phone has a smart notification filter that classifies notifications into:
- **"Important"** → If it is from "Bank", "Emergency Services", or "Government"  
- **"Social"** → If it is from "Facebook", "Instagram", or "Twitter"  
- **"Work"** → If it is from "Boss", "HR", or "Team"  
- **"Other"** → For anything else  

Take the sender name as input and determine the category of the notification.  

#### Sample Test Cases:  
##### Test Case 1:  
**Input:**  
```
sender = "Bank"
```  
**Output:**  
```
Important
```  
**Explanation:** Since the sender is "Bank", it is an important notification.  

##### Test Case 2:  
**Input:**  
```
sender = "HR"
```  
**Output:**  
```
Work
```  
**Explanation:** "HR" falls under the work category.  

---

### 4. Digital Lock Access  
#### Problem:  
A **digital lock** grants access based on the entered **4-digit passcode** and additional conditions:  
- If the passcode **starts with "9"**, allow access with "Admin Access Granted"  
- If the passcode **starts with "1" or "2"**, allow access with "User Access Granted"  
- If the passcode **ends with "0"**, allow access with "Guest Access Granted"  
- Otherwise, deny access with "Access Denied"  

#### Sample Test Cases:  
##### Test Case 1:  
**Input:**  
```
passcode = "9123"
```  
**Output:**  
```
Admin Access Granted
```  
**Explanation:** The passcode starts with "9", so admin access is granted.  

##### Test Case 2:  
**Input:**  
```
passcode = "5670"
```  
**Output:**  
```
Guest Access Granted
```  
**Explanation:** The passcode ends with "0", so guest access is granted.  

---

### 5. Smart Music Player Mode  
#### Problem:  
A **smart music player** changes its playback mode based on the genre of the current song:  
- **"Party Mode"** → If the song is **Pop, EDM, or Dance**  
- **"Relax Mode"** → If the song is **Classical, Jazz, or Acoustic**  
- **"Workout Mode"** → If the song is **Rock, Hip-Hop, or Metal**  
- **"Default Mode"** → For any other genre  

Take the **genre** of a song as input and determine the playback mode.  

#### Sample Test Cases:  
##### Test Case 1:  
**Input:**  
```
genre = "EDM"
```  
**Output:**  
```
Party Mode
```  
**Explanation:** "EDM" falls under party mode.  

##### Test Case 2:  
**Input:**  
```
genre = "Jazz"
```  
**Output:**  
```
Relax Mode
```  
**Explanation:** "Jazz" falls under relax mode.  

##### Test Case 3:  
**Input:**  
```
genre = "Rock"
```  
**Output:**  
```
Workout Mode
```  
**Explanation:** "Rock" falls under workout mode.  

##### Test Case 4:  
**Input:**  
```
genre = "Country"
```  
**Output:**  
```
Default Mode
```  
**Explanation:** "Country" does not belong to any predefined category, so default mode is selected.  

---

### 6. Automated Email Response
#### Problem:
An email system automatically responds based on the subject line:
- **"Out of Office"** → If the subject contains "leave", "vacation", or "holiday".
- **"Urgent Response Required"** → If the subject contains "urgent" or "ASAP".
- **"General Inquiry"** → If the subject contains "help", "question", or "support".
- **"No Action Needed"** → For any other subject.

#### Sample Test Cases:
##### Test Case 1:
**Input:**
```
subject = "I am on vacation next week"
```
**Output:**
```
Out of Office
```
**Explanation:** The subject contains "vacation", so an out-of-office reply is sent.

##### Test Case 2:
**Input:**
```
subject = "Need support with my account"
```
**Output:**
```
General Inquiry
```
**Explanation:** The subject contains "support", so it is classified as a general inquiry.

---

### 7. Smart Car Mode Selection
#### Problem:
A smart car adjusts its mode based on the driving condition:
- **"Eco Mode"** → If the fuel level is below 20% and speed is under 60 km/h.
- **"Sport Mode"** → If speed is above 100 km/h.
- **"Comfort Mode"** → If the air conditioning is on and speed is between 60-100 km/h.
- **"Normal Mode"** → For any other condition.

#### Sample Test Cases:
##### Test Case 1:
**Input:**
```
fuel = 15
speed = 50
ac = False
```
**Output:**
```
Eco Mode
```
**Explanation:** Fuel level is below 20% and speed is under 60 km/h, so Eco Mode is selected.

##### Test Case 2:
**Input:**
```
fuel = 40
speed = 110
ac = True
```
**Output:**
```
Sport Mode
```
**Explanation:** Speed is above 100 km/h, so Sport Mode is selected.

---

### 8. Smart Security Camera Detection
#### Problem:
A security camera identifies objects and takes action accordingly:
- **"Alert: Intruder Detected"** → If the detected object is "Person" at night.
- **"Animal Detected"** → If the object is "Dog", "Cat", or "Bird".
- **"Vehicle Detected"** → If the object is "Car" or "Bike".
- **"No Threat Detected"** → For any other object.

#### Sample Test Cases:
##### Test Case 1:
**Input:**
```
object_detected = "Person"
time = "23:00"
```
**Output:**
```
Alert: Intruder Detected
```
**Explanation:** Since a person is detected at night, an intruder alert is triggered.

##### Test Case 2:
**Input:**
```
object_detected = "Dog"
time = "14:30"
```
**Output:**
```
Animal Detected
```
**Explanation:** The object detected is a dog, so it falls under the "Animal Detected" category.

---

