## 01. Hollow Diamond

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/hollow-diamond/1)

### Problem Description

**Task:** Given a number n. Print Hollow Diamond Pattern with n lines.

> **Note:** There is a space between two adjacent stars (*) in the pattern.

#### Examples

##### Example 1

- **Input:**
```text
n = 3Output: * * ** * * * *
```

##### Example 2

- **Input:**
```text
n = 5Output: * * * * * * ** * * * * * * * *
```

#### Constraints

- **1.** `1 ≤ n ≤ 100`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-06-13 09:20:56
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def printPat(self, n):
        # code here
        for i in range(1,n+1):
            spaces=" "*(2*(n-i))
            if i==1:
                print(spaces+"*")
            else:
                midspace=" "*(4*i-5)
                print(spaces+"*"+midspace+"*")
            
        for i in range(n-1,0,-1):
            spaces=" "*(2*(n-i))
            if i==1:
                print(spaces+"*")
            else:
                midspace=" "*(4*i-5)
                print(spaces+"*"+midspace+"*")
```

*Generated on: 9/28/2026, 12:41:36 AM*