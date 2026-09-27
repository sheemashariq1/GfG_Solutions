## 01. Max Circular Subarray Sum

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/max-circular-subarray-sum-1587115620/1)

### Problem Description

**Task:** You are given a circular array arr[] of integers, find the maximum possible sum of a non-empty subarray. In a circular array, the subarray can start at the end and wrap around to the beginning. Return the maximum non-empty subarray sum, considering both non-wrapping and wrapping cases.Examples:Input: arr[] = [8, -8, 9, -9, 10, -11, 12]

#### Examples

##### Example 1

- **Output:**
```text
23
```
- **Explanation:** The circular subarray [3, 4, 5] gives the maximum sum of 12.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-20 11:18:10
- **Status:** Correct
- **Marks:** 8

```cpp
class Solution {
  public:
    int maxCircularSum(vector<int> &arr) {
        // code here
        int sum=arr[0];
        int max1=arr[0];
        int max_end=arr[0];
        int min1=arr[0];
        int min_end=arr[0];
        for(int i=1;i<arr.size();i++){
            sum+=arr[i];
            max_end=max(arr[i],max_end+arr[i]);
            max1=max(max1,max_end);
            min_end=min(arr[i],min_end+arr[i]);
            min1=min(min1,min_end);
        }
        if(max1<0){
            return max1;
        }
        return max(max1,sum-min1);
    }
};
```

*Generated on: 9/28/2026, 12:11:54 AM*