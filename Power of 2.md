## 01. Power of 2

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/power-of-2-1587115620/1)

### Problem Description

**Task:** Given a non-negative integer n, return true if it is a power of 2. Otherwise, return false. ExamplesInput: n = 8

#### Examples

##### Example 1

- **Output:**
```text
true
```
- **Explanation:** (2⁰ = 1).

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-25 14:43:30
- **Status:** Correct
- **Marks:** 2

```cpp
class Solution {
  public:
    bool isPowerofTwo(int n) {
        // code here
        return (n>0) &&((n&(n-1))==0);
    }
};
```

*Generated on: 9/28/2026, 12:31:10 AM*