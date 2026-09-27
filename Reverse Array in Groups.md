## 01. Reverse Array in Groups

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/reverse-array-in-groups0255/1)

### Problem Description

**Task:** Given an integer array arr[] and an integer k, reverse every consecutive group of k elements. If fewer than k elements remain at the end, reverse all of them.Examples:Input: arr[] = [1, 2, 3, 4, 5], k = 3Output: [3, 2, 1, 5, 4]

#### Examples

##### Example 1

- **Explanation:** First group consists of elements 1, 2, 3. Second group consists of 4, 5.Input: arr[] = [5, 6, 8, 9], k = 5Output: [9, 8, 6, 5]Explnation: Since k is greater than the number of remaining elements, the entire array is reversed.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-16 11:00:13
- **Status:** Correct
- **Marks:** 4

```cpp
class Solution {
  public:
    void reverseInGroups(vector<int> &arr, int k) {
        // code here
    for(int i=0;i<arr.size();i+=k){
        int left=i;
        int right=min(i+k-1,(int)arr.size()-1);
        while(left<right){
            swap(arr[left],arr[right]);
            left++;
            right--;
        }
    }
    }
};
```

*Generated on: 9/28/2026, 12:40:16 AM*