## 01. Print Number Pattern

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/print-the-pattern-set-1/1)

### Problem Description

**Task:** You are given a number n. You need to generate and print a pattern based on the given value of n.For each row, starting from the first, print numbers in descending order from n down to 1.Each number in a row is repeated as many times as the current row index (starting from n).Instead of printing each row on a new line, separate rows with -1.Instead of a newline at the end of each row, print -1 to indicate row separation. After printing the entire pattern, end the output with -1.For n = 3,pattern: 3 3 3 2 2 2 1 1 1 3 3 2 2 1 1 3 2 1For n = 2,pattern: 2 2 1 1 2 1Examples :Input: 2

#### Examples

##### Example 1

- **Output:**
```text
[1, -1]
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(n^2)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-09 12:15:01
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    vector<int> printPat(int n) {
        vector<int> result;

        for (int i = n; i >= 1; i--) {
            // Each number j repeated i times
            for (int j = n; j >= 1; j--) {
                for (int k = 1; k <= i; k++) {
                    result.push_back(j);
                }
            }
            result.push_back(-1);
        }

        return result;
    }
};
```

*Generated on: 9/28/2026, 12:46:19 AM*