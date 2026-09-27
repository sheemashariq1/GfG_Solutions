## 01. Print n to 1 Without Loop

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/print-n-to-1-without-loop/1)

### Problem Description

**Task:** Given an integer n, print all numbers from n to 1 in decreasing order, separated by spaces, without using any loops.Examples :Input: n = 5

#### Examples

##### Example 1

- **Output:**
```text
3 2 1
```
- **Explanation:** The numbers from 3 to 1 are printed in decreasing order

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (2)

#### Solution 1 (Python)

- **Submitted:** 2026-06-11 11:47:15
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def printNos(self, n):
        # Code here
        if n<1:
            return
        print(n,end=" ")
        self.printNos(n-1)
```

#### Solution 2 (Python)

- **Submitted:** 2026-06-11 11:45:58
- **Status:** Correct
- **Marks:** 2

```python
class Solution {
  public:
    void printNos(int n) {
        // code here
        if(n<1)
        {
            return;
        }
        cout<<n<<" ";
        printNos(n-1);
    }
};
```

*Generated on: 9/28/2026, 12:42:48 AM*