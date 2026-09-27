## 01. Sum of Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/sum-all-array-elements/1)

### Problem Description

**Task:** Given an integer array arr[], return the sum of all elements of arr.Examples:Input: arr[] = [1, 2, 3, 4]

#### Examples

##### Example 1

- **Output:**
```text
10
```
- **Explanation:** 1 + 2 + 3 + 4 = 10.

##### Example 2

- **Input:**
```text
arr[] = [1, 3, 3]
```
- **Output:**
```text
7
```
- **Explanation:** 1 + 3 + 3 = 7.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (C++)

- **Submitted:** 2026-06-30 12:12:13
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution {
  public:
  int sum_of_array(vector<int> &arr,int element){
      if(element==arr.size()){
          return 0;
      }
      return arr[element] + sum_of_array(arr,element+1);
  }
    int arraySum(vector<int>& arr) {
        // code here
        return sum_of_array(arr,0);
    }
};
```

#### Solution 2 (C++)

- **Submitted:** 2026-06-08 12:08:20
- **Status:** Correct
- **Marks:** 2

```cpp
class Solution {
  public:
    int arraySum(vector<int>& arr) {
        // code here
        int sum=0;
        for(int num:arr){
            sum+=num;
        }
        return sum;
    }
};
```

*Generated on: 9/28/2026, 12:48:15 AM*