## 01. Median of 2 Sorted Arrays of Same Size

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/median-of-2-sorted-arrays-of-same-size/1)

### Problem Description

**Task:** Given two sorted arrays a[] and b[] of equal size, find and return the median of the combined array after merging them into a single sorted array.

#### Examples

##### Example 1

- **Input:**
```text
a[] = [-5, 3, 6, 12, 15], b[] = [-12, -10, -6, -3, 4]
```
- **Output:**
```text
0
```
- **Explanation:** The merged array is [-12, -10, -6, -5, -3, 3, 4, 6, 12, 15]. So the median of the merged array is (-3 + 3) / 2 = 0.

##### Example 2

- **Input:**
```text
a[] = [2, 3, 5, 7], b[] = [10, 12, 14, 16]Output: 8.5Explanation: The merged array is [2, 3, 5, 7, 10, 12, 14, 16]. So the median of the merged array is (7 + 10) / 2 = 8.5.
```

##### Example 3

- **Input:**
```text
a[] = [-5], b[] = [-6]
```
- **Output:**
```text
-5.5Explanation: The merged array is [-6, -5]. So the median of the merged array is (-6 + -5) / 2 = -5.5.
```

#### Constraints

- **1.** `1 ≤ a.size(), b.size() ≤ 10⁶-10⁶ ≤ a[i], b[i] ≤ 10⁶`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-22 15:47:50
- **Status:** Correct
- **Marks:** 8

```cpp
class Solution {
  public:
    double medianOf2(vector<int>& a, vector<int>& b) {
        // Your code goes here
        int n=a.size();
        vector<int> merged(2*n);
        merge(a.begin(),a.end(),b.begin(),b.end(),merged.begin());
        return (merged[n-1]+merged[n])/2.0;
    }
};
```

*Generated on: 9/28/2026, 12:07:18 AM*