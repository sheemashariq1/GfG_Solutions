## 01. Largest in Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/largest-element-in-array4009/1)

### Problem Description

**Task:** Given an array arr[]. The task is to find the largest element and return it.Examples:Input: arr[] = [1, 8, 7, 56, 90]

#### Examples

##### Example 1

- **Output:**
```text
10
```
- **Explanation:** There is only one element which is the largest.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-20 11:46:44
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    int largest(vector<int> &arr) {
        // code here
        int max1=arr[0];
        for(int i=1;i<arr.size();i++){
            if(arr[i]>max1){
                max1=arr[i];
            }
        }
        return max1;
    }
};
```

*Generated on: 9/28/2026, 12:37:11 AM*