## 01. GCD of Two

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/gcd-of-two-numbers3459/1)

### Problem Description

**Task:** Given two positive integers a and b, find GCD of a and b.

> **Note:** Don't use the inbuilt gcd function

#### Examples

##### Example 1

- **Input:**
```text
a = 20, b = 28
```
- **Output:**
```text
4
```
- **Explanation:** GCD of 20 and 28 is 4

##### Example 2

- **Input:**
```text
a = 60, b = 36
```
- **Output:**
```text
12
```
- **Explanation:** GCD of 60 and 36 is 12

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log(min(a, b)))
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (Python)

- **Submitted:** 2026-06-12 11:54:23
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def gcd(self, a, b):
        # code here
        if b==0:
            return a
        return self.gcd(b,a%b)
```

#### Solution 2 (Python)

- **Submitted:** 2026-06-12 11:51:41
- **Status:** Correct
- **Marks:** 1

```python
class Solution {
  public:
    int gcd(int a, int b) {
        // code here
        if(b==0){
            return a;
        }
        return gcd(b,a%b);
    }
};
```

*Generated on: 9/28/2026, 12:42:02 AM*