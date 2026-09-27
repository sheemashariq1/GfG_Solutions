## 01. Decision Making

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/decision-making/1)

### Problem Description

**Task:** Given two integers, n and m. The task is to check the relation between n and m. Print "less" if n < m, "equal" if n = = m, and "greater" if n > m.

#### Examples

##### Example 1

- **Input:**
```text
n = 4, m = 8
```
- **Output:**
```text
less
```
- **Explanation:** 4 < 8 so print 'less'.

##### Example 2

- **Input:**
```text
n = 8, m = 8
```
- **Output:**
```text
equal
```
- **Explanation:** 8 = 8 so print 'equal'.

##### Example 3

- **Input:**
```text
n = 8, m = 4
```
- **Output:**
```text
greater
```
- **Explanation:** 8 > 4 so print 'greater'.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-09-11 23:25:31
- **Status:** Correct
- **Marks:** 1

```python
n = int(input())
m = int(input())

# code here
if n<m:
    print("less")
elif n==m:
    print("equal")
else:
    print("greater")
```

*Generated on: 9/28/2026, 12:20:32 AM*