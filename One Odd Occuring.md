## 01. One Odd Occuring

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/find-the-odd-occurence4820/1)

### Problem Description

**Task:** Given an array of arr[] positive integers where all numbers occur even number of times except one number which occurs odd number of times. Return that number.Examples:Input:arr[] = [1, 2, 3, 2, 3, 1, 3]

#### Examples

##### Example 1

- **Output:**
```text
3
```
- **Explanation:** 3 occurs three times.

##### Example 2

- **Input:**
```text
arr[] = [5, 7, 2, 7, 5, 2, 5]
```
- **Output:**
```text
5
```
- **Explanation:** 5 occurs three times.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-26 15:37:54
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    int getOddOccurrence(vector<int>& arr) {
        // code here
        int res=0;
        for(int num:arr){
            res^=num;
        }
        return res;
    }
};
```

*Generated on: 9/28/2026, 12:27:00 AM*