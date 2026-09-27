## 01. Leap Year

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/leap-year0943/1)

### Problem Description

**Task:** You are given an Integer n. Return true if It is a Leap Year otherwise return false.

#### Examples

##### Example 1

- **Input:**
```text
n = 4
```
- **Output:**
```text
true
```
- **Explanation:** 4 is not divisible by 100 and is divisible by 4 so its a leap year

##### Example 2

- **Input:**
```text
n = 2021
```
- **Output:**
```text
false
```
- **Explanation:** 2021 is not divisible by 100 and is also not divisible by 4 so its not a leap year

#### Constraints

- **1.** `1 <= n < 10⁴`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-07 13:40:55
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    bool checkYear(int n) {
        // code here
        if ((n%400==0) ||(n%4==0 && n%100!=0))
        {
            return true;
        }
        else
        {
            return false;
        }
    }
};
```

*Generated on: 9/28/2026, 12:50:57 AM*