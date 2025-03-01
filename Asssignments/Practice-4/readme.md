**Python Practice Exercises**

---

#### **Problem 1: Supermarket Cart Management**  
A supermarket uses a list to store items added to a cart. Given a list of items, perform the following operations:  
- Replace the first item with "Milk".  
- Remove the last item.  
- Reverse the list.  
- Extract the first 3 items.  

##### **Sample Test Case**  
**Input:**  
```python
cart = ["Apples", "Bananas", "Grapes", "Chocolates"]
```
**Output:**  
```python
['Milk', 'Bananas', 'Grapes']
```
**Explanation:**  
- First item replaced.
- Last item removed.
- List reversed.
- Extracted first 3 items.  

---

#### **Problem 2: Playlist Organizer**  
A music app maintains a list of songs. Given a list of songs, perform the following operations:  
- Add a new song at the end.  
- Remove the second song.  
- Extract the last 2 songs.  

##### **Sample Test Case**  
**Input:**  
```python
songs = ["Song1", "Song2", "Song3", "Song4"]
new_song = "Song5"
```
**Output:**  
```python
['Song3', 'Song4', 'Song5']
```

---

#### **Problem 3: GPS Coordinates**  
A GPS tracker stores the location of a traveler as a tuple `(latitude, longitude, altitude)`. Extract latitude, longitude, and convert altitude to meters.  

##### **Sample Test Case**  
**Input:**  
```python
location = (17.3850, 78.4867, 2.1)  
```
**Output:**  
```python
(17.3850, 78.4867, 2100)
```

---

#### **Problem 4: Student Attendance**  
Two classes attended a workshop. Given two sets of roll numbers, find:
- Students in both classes.
- Students unique to Class A.
- Total unique students.

##### **Sample Test Case**  
**Input:**  
```python
class_A = {101, 102, 103, 104, 105}
class_B = {103, 104, 106, 107}
```
**Output:**  
```python
Common: {103, 104}
Only A: {101, 102, 105}
Total unique: {101, 102, 103, 104, 105, 106, 107}
```

---

#### **Problem 5: Email Username Extractor**  
Extract the username from an email ID and convert it to uppercase.

##### **Sample Test Case**  
**Input:**  
```python
email = "john.doe@example.com"
```
**Output:**  
```python
"JOHN.DOE"
```

---

#### **Problem 6: Bakery Profit Calculation**  
A bakery sells cupcakes and cookies. Given their count, calculate total revenue and compare earnings.

##### **Sample Test Case**  
**Input:**  
```python
cupcakes = 10
cookies = 15
```
**Output:**  
```python
Total revenue: ₹950
Cupcakes earned ₹200 more than cookies.
```

---

#### **Problem 7: Sentence Reversal**  
Given a sentence, reverse the words while maintaining their case.

##### **Sample Test Case**  
**Input:**  
```python
sentence = "Python is awesome"
```
**Output:**  
```python
"awesome is Python"
```

---

#### **Problem 8: Favorite Fruits**  
Two friends list their favorite fruits. Find:
- Common fruits.
- Unique fruits to friend1.
- Total different fruits.

##### **Sample Test Case**  
**Input:**  
```python
friend1 = {"Apple", "Banana", "Grapes"}
friend2 = {"Grapes", "Mango", "Orange"}
```
**Output:**  
```python
Common: {'Grapes'}
Only friend1: {'Apple', 'Banana'}
Total unique: {'Apple', 'Banana', 'Grapes', 'Mango', 'Orange'}
```

---

#### **Problem 9: Movie Ratings**  
A streaming platform stores movies and their ratings as tuples `(movie_name, rating)`. Given a tuple of movies, extract:
- The movie with the highest rating.
- The first 3 movies.

##### **Sample Test Case**  
**Input:**  
```python
movies = [("Inception", 9.0), ("Titanic", 8.8), ("Avatar", 7.9), ("Interstellar", 9.2)]
```
**Output:**  
```python
('Interstellar', 9.2)
[("Inception", 9.0), ("Titanic", 8.8), ("Avatar", 7.9)]
```

---

#### **Problem 10: Shopping Discounts**  
A store offers a discount on purchases above ₹500. Given the total bill, determine the final amount after discount.

##### **Sample Test Case**  
**Input:**  
```python
bill = 600
discount = 10  # 10% discount
```
**Output:**  
```python
Final Amount: ₹540
```

---

**Python Complex Practice Problems**

---

### **Problem 11: Stock Market Analysis**  
A stock trader wants to analyze daily stock prices. Given a list of stock prices, perform the following:
- Find the maximum and minimum stock price.
- Calculate the difference between the highest and lowest price.
- Return the sorted list of stock prices.

##### **Sample Test Case**  
**Input:**  
```python
prices = [150, 200, 250, 180, 300, 220]
```
**Output:**  
```python
Max Price: 300
Min Price: 150
Difference: 150
Sorted Prices: [150, 180, 200, 220, 250, 300]
```

---

### **Problem 12: Social Media Engagement Calculation**  
A social media app tracks engagement using likes and comments per post. Given a list of tuples representing post engagements:
- Compute total engagement for each post.
- Find the post with the highest engagement.
- Return a sorted list of total engagements.

##### **Sample Test Case**  
**Input:**  
```python
posts = [("Post1", 150, 30), ("Post2", 200, 50), ("Post3", 120, 20), ("Post4", 180, 40)]
```
**Output:**  
```python
Total Engagements: [180, 250, 140, 220]
Most Engaging Post: Post2
Sorted Engagements: [140, 180, 220, 250]
```

---

### **Problem 13: Movie Ratings Processing**  
A survey collects ratings for movies. Given a list of movie ratings, perform the following:
- Find the highest and lowest ratings.
- Calculate the sum of all ratings.
- Compute the average rating.

##### **Sample Test Case**  
**Input:**  
```python
ratings = [9.0, 8.8, 7.9, 9.2, 8.5]
```
**Output:**  
```python
Highest Rating: 9.2
Lowest Rating: 7.9
Total Rating: 43.4
Average Rating: 8.68
```

---

