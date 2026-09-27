## 01. Size of an Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/size-of-an-array/1)

### Problem Description

**Task:** Given an array arr[], find the size of the array.Examples :Input: arr[] = [1, 2, 3]

#### Examples

##### Example 1

- **Output:**
```text
5
```
- **Explanation:** The size of the array is 5.Constraints:1 ≤ |arr| ≤ 101 ≤ elements of arr ≤ 10

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-08-08 12:30:11
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    int getSize(vector<int>& arr) {
        // code here
        return arr.size();
    }
};
```

*Generated on: 9/28/2026, 12:26:02 AM*