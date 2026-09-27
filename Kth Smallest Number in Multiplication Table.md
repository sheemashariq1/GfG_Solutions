## 01. Kth Smallest Number in Multiplication Table

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/kth-smallest-number-in-multiplication-table/1)

### Problem Description

**Task:** Given three integers n, m and k. Consider a grid of n * m, where mat[i][j] = i * j (1 based index). The task is to return the k^th smallest element in the n * m multiplication table.

#### Examples

##### Example 1

- **Input:**
```text
n = 3, m = 5, k = 7
```
- **Output:**
```text
4 Sorted form of all the element of this matrix is [1, 2, 2, 3, 3, 4, 4, 5, 6, 6, 8, 9, 10, 12, 15] and the 7th smallest element is 4.
```

##### Example 2

- **Input:**
```text
n = 2, m = 2, k = 3
```
- **Output:**
```text
2Explanation: Sorted form of all the element of this matrix is [1, 2, 2, 4] and 3rd smallest element is 2.
```

#### Constraints

- **1.** `1 ≤ n, m ≤ 3 * 10⁴¹ ≤ k ≤ n * m`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n * log (n*m))
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-22 15:27:18
- **Status:** Correct
- **Marks:** 8

```cpp
class Solution {
  public:
    int kthSmallest(int n, int m, int k) {
        // code here
        int low=1;
        int high=n*m;
        int ans=high;
        while(low<=high){
            int mid=low+(high-low)/2;
            int count=0;
            for(int i=1;i<=n;i++){
                count+=min(mid/i,m);
            }
            if(count>=k){
                ans=mid;
                high=mid-1;
            }
            else{
                low=mid+1;
            }
        }
        return ans;
    }
};
```

*Generated on: 9/28/2026, 12:10:37 AM*