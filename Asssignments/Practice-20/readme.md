## Problem 1: Alternating Sum

### Description
Given a list of integers, compute an alternating sum by adding elements at even indices and subtracting elements at odd indices.

### Example
**Input:**
```
[5, 3, 8, 1, 4]
```
**Output:**
```
13
```
**Explanation:**
5 - 3 + 8 - 1 + 4 = 13

## Problem 2: Consecutive Pairs

### Description
Given a list of integers, find the number of consecutive pairs where the second element is greater than the first.

### Example
**Input:**
```
[1, 3, 2, 5, 4, 7]
```
**Output:**
```
3
```
**Explanation:**
Pairs (1,3), (2,5), and (4,7) all have the second number greater than the first.

## Problem 3: Peak Finder

### Description
Find all peak elements in a list. A peak element is greater than both of its neighbors. First and last elements can be peaks if they are greater than their only neighbor.

### Example
**Input:**
```
[1, 3, 2, 5, 3, 9, 8]
```
**Output:**
```
[3, 5, 9]
```
**Explanation:**
3 is greater than 1 and 2
5 is greater than 2 and 3
9 is greater than 3 and 8

## Problem 4: Running Sum with Threshold

### Description
Given a list of integers and a threshold value, create a new list where each element is the running sum of the original list, but reset to zero whenever the running sum exceeds the threshold.

### Example
**Input:**
```
[3, 2, 5, 1, 7, 3, 4], threshold=8
```
**Output:**
```
[3, 5, 0, 1, 0, 3, 7]
```
**Explanation:**
Running sum starts at 3
3+2=5, still under threshold
5+5=10, exceeds threshold, reset to 0
0+1=1, under threshold
1+7=8, equals threshold (not exceeding), so keep it
8+3=11, exceeds threshold, reset to 0
0+3=3, under threshold
3+4=7, final element

## Problem 5: Longest Increasing Subsequence

### Description
Find the length of the longest strictly increasing subsequence of consecutive elements in a list.

### Example
**Input:**
```
[1, 3, 5, 4, 7, 8, 9, 3]
```
**Output:**
```
4
```
**Explanation:**
The longest increasing subsequence of consecutive elements is [4, 7, 8, 9] with length 4.

## Problem 6: Group Alternating Elements

### Description
Given a list, create a new list where elements at even indices form the first part, and elements at odd indices form the second part.

### Example
**Input:**
```
['a', 'b', 'c', 'd', 'e', 'f']
```
**Output:**
```
['a', 'c', 'e', 'b', 'd', 'f']
```
**Explanation:**
First part: elements at indices 0, 2, 4 ('a', 'c', 'e')
Second part: elements at indices 1, 3, 5 ('b', 'd', 'f')

## Problem 7: Sum Between Zeros

### Description
Given a list of integers, calculate the sum of elements between each pair of zeros. Return a list of these sums.

### Example
**Input:**
```
[0, 3, 5, 0, 2, 4, 0, 1, 0]
```
**Output:**
```
[8, 6, 1]
```
**Explanation:**
Sum between first two zeros: 3+5=8
Sum between next two zeros: 2+4=6
Sum between last two zeros: 1

## Problem 8: Filter by Neighbors

### Description
Create a list containing only elements which are greater than at least one of their neighboring elements.

### Example
**Input:**
```
[5, 3, 8, 2, 5, 4, 7]
```
**Output:**
```
[5, 8, 5, 7]
```
**Explanation:**
5 > 3 (its right neighbor)
8 > 3 and 8 > 2 (both neighbors)
5 > 2 (its left neighbor)
7 > 4 (its left neighbor)

## Problem 9: Stepping Stones

### Description
Determine if you can reach the end of a list starting from index 0, where each value represents the maximum number of steps you can take forward at that position.

### Example
**Input:**
```
[3, 1, 0, 2, 4]
```
**Output:**
```
True
```
**Explanation:**
Start at index 0 with value 3
Can jump to indices 1, 2, or 3
Jump to index 3 with value 2
Can jump to index 4 or 5
Jump to index 5, which is past the end, so we can reach the end

**Input:**
```
[2, 0, 1, 0]
```
**Output:**
```
False
```
**Explanation:**
Start at index 0 with value 2
Can jump to indices 1 or 2
If jump to index 1, stuck with 0 steps
If jump to index 2, can only move 1 step to index 3
At index 3, stuck with 0 steps, can't reach the end

## Problem 10: Pattern Matching Counter

### Description
Count occurrences of a specific pattern in a list. A pattern is a consecutive sequence of elements.

### Example
**Input:**
```
List: [1, 2, 3, 1, 2, 1, 2, 3], Pattern: [1, 2]
```
**Output:**
```
3
```
**Explanation:**
Pattern [1, 2] occurs at positions 0, 3, and 5

## Problem 11: Balance Point

### Description
Find the index where the sum of elements to the left equals the sum of elements to the right. If there's no such index, return -1.

### Example
**Input:**
```
[1, 7, 3, 6, 5, 6]
```
**Output:**
```
3
```
**Explanation:**
At index 3: Sum of left elements (1+7+3) = 11, Sum of right elements (5+6) = 11

**Input:**
```
[1, 2, 3, 4, 6]
```
**Output:**
```
-1
```
**Explanation:**
No index has equal sum on both sides

## Problem 12: Zigzag Conversion

### Description
Transform a list into a zigzag pattern. If the zigzag has `n` rows, then the elements should be read row by row.

### Example
**Input:**
```
List: [1, 2, 3, 4, 5, 6, 7, 8, 9], Rows: 3
```
**Output:**
```
[1, 5, 9, 2, 4, 6, 8, 3, 7]
```
**Explanation:**
The zigzag looks like:
```
1   5   9
 2 4 6 8
  3   7
```
Reading by rows gives [1, 5, 9, 2, 4, 6, 8, 3, 7]

## Problem 13: Majority Element

### Description
Find the majority element in a list (an element appearing more than n/2 times, where n is the length of the list). You can assume the majority element always exists.

### Example
**Input:**
```
[3, 2, 3, 2, 3, 1, 3]
```
**Output:**
```
3
```
**Explanation:**
3 appears 4 times, which is more than 7/2 = 3.5 times

## Problem 14: Sliding Window Maximum

### Description
Given a list of integers and a window size k, find the maximum element in each consecutive window of size k.

### Example
**Input:**
```
List: [1, 3, -1, -3, 5, 3, 6, 7], Window size: 3
```
**Output:**
```
[3, 3, 5, 5, 6, 7]
```
**Explanation:**
Window 1 [1, 3, -1]: max is 3
Window 2 [3, -1, -3]: max is 3
Window 3 [-1, -3, 5]: max is 5
Window 4 [-3, 5, 3]: max is 5
Window 5 [5, 3, 6]: max is 6
Window 6 [3, 6, 7]: max is 7

## Problem 15: Jump Game

### Description
Given a list of non-negative integers, you are initially positioned at the first index. Each element represents the maximum jump length at that position. Determine if you can reach the last index.

### Example
**Input:**
```
[2, 3, 1, 1, 4]
```
**Output:**
```
True
```
**Explanation:**
Jump 1 step from index 0 to index 1, then 3 steps to the last index.

**Input:**
```
[3, 2, 1, 0, 4]
```
**Output:**
```
False
```
**Explanation:**
You will always arrive at index 3 with value 0, which means you cannot jump to the last index.
