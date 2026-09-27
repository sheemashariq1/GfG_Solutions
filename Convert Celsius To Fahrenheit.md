## 01. Convert Celsius To Fahrenheit

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/convert-celsius-to-fahrenheit/1)

### Problem Description

**Task:** Given a temperature in celsius C. You need to convert the given temperature into Fahrenheit.

#### Examples

##### Example 1

- **Input:**
```text
C = 32
```
- **Output:**
```text
89.6
```
- **Explanation:** Using the conversion formula of celsius to farhenheit , it can be calculated that, for 32 degree celsius, the temperature in Fahrenheit = 89.6

##### Example 2

- **Input:**
```text
C = 50
```
- **Output:**
```text
122
```
- **Explanation:** Using the conversion formula of celsius to farhenheit, it can be calculated that, for 50 degree C, the temperature in Fahrenheit = 122.

#### Constraints

- **1.** `1 ≤ C ≤ 10⁴`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-07 13:24:53
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    double cToF(int C) {
        // code here
        return (C*9/5)+32;
    }
};
```

*Generated on: 9/28/2026, 12:52:19 AM*