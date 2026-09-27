## 01. Array Subset

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/array-subset-of-another-array2317/1)

### Problem Description

**Task:** Given two arrays a[] and b[], your task is to determine whether b[] is a subset of a[].Examples:Input: a[] = [11, 7, 1, 13, 21, 3, 7, 3], b[] = [11, 3, 7, 1, 7]

#### Examples

##### Example 1

- **Output:**
```text
false
```
- **Explanation:** b[] is not a subset of a[]

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n + m)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-27 15:29:12
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    // Function to check if b is a subset of a
    bool isSubset(vector<int> &a, vector<int> &b) {
        // Your code here
        unordered_map<int,int> freq;
        for(int num:a){
            freq[num]++;
        }
        for(int num:b){
            if(freq[num]==0){
                return false;
            }
            freq[num]--;
        }
        return true;
    }
};
```

*Generated on: 9/28/2026, 12:27:45 AM*