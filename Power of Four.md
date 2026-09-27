## 01. Power of Four

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/power-of-four/1)

### Problem Description

**Task:** Given a number n, check if n is power of 4 or not.

#### Examples

##### Example 1

- **Input:**
```text
n = 64
```
- **Output:**
```text
true
```
- **Explanation:** 4³ = 64

##### Example 2

- **Input:**
```text
n = 75
```
- **Output:**
```text
false
```
- **Explanation:** 75 is not a power of 4.

#### Constraints

- **1.** `1 ≤ n ≤ 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-25 14:56:46
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    bool isPowerOfFour(int n){
        // code here
        return(n>0) && ((n&(n-1))==0) && (n& 0x55555555);
    }
    };
```

*Generated on: 9/28/2026, 12:29:12 AM*