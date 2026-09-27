## 01. Taking Input

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/taking-input/1)

### Problem Description

**Task:** You need to perform three separate tasks based on the given input:
String Input and Print: Read a string s (which may contain spaces) and print it as it is.
Integer Input and Print: Read an integer n and print it without any change.
Float Input and floor Print: Read a floating-point number as input, take its floor value, and print as an integer.

#### Examples

##### Example 1

- **Input:**
```text
s = "Hello", n = 20, f = 5.5Output: Hello 20 5Explanation: The string Hello is printed as it is. The integer 20 is printed without any change.For floating-point number 5.5, its floor value 5 is printed.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-09-11 23:32:47
- **Status:** Correct
- **Marks:** 1

```python
import math

# s to store string
# n to store integer
# f to store float
# ff  # To Store floor of float variable f

# code here
s = input()
n = int(input())
f = float(input())

ff = math.floor(f)

print(s)
print(n)
print(ff)
```

*Generated on: 9/28/2026, 12:17:09 AM*