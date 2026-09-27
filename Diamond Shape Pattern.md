## 01. Diamond Shape Pattern

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/pattern/1)

### Problem Description

**Task:** Given a number n, print a diamond-shaped star pattern with 2n rows, where the number of stars first increases and then decreases to form the diamond.

#### Examples

##### Example 1

- **Input:**
```text
n = 5Output:
```

##### Example 2

- **Input:**
```text
n = 3Output: * * ** * ** * * * * *
```

#### Constraints

- **1.** `1 ≤ n ≤ 100`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-09 11:33:09
- **Status:** Correct
- **Marks:** 4

```cpp
class Solution {
  public:
    void printDiamond(int n) {
        // code here
     for (int i = 1; i <= n; i++) {
            for (int j = i; j < n; j++) {
                cout << " ";
            }
            for (int j = 1; j <= i; j++) {
                cout << "* ";
            }
            cout << "\n";
        }
        for (int i = n; i >= 1; i--) {
            for (int j = i; j < n; j++) {
                cout << " ";
            }
            for (int j = 1; j <= i; j++) {
                cout << "* ";
            }
             cout << "\n";
         }
    } 
};
```

*Generated on: 9/28/2026, 12:47:22 AM*