## 01. Print Hollow Rectangle

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/hollow-rectangle-or-square/1)

### Problem Description

**Task:** Given two integers n and m, print a hollow rectangle pattern consisting of n rows and m columns.Examples:Input: n = 3, m = 5Output:****** ******Input: n = 4, m = 3Output:**** ** * ***

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n * m)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (Python)

- **Submitted:** 2026-06-09 13:22:15
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def printHollowRect(self, n, m):
        # code here
        for i  in range(1,n+1):
            for j in range(1,m+1):
                if i==1 or i==n or j==1 or j==m:
                    print("*",end="")
                else:
                    print(" ",end="")
            print()
```

#### Solution 2 (Python)

- **Submitted:** 2026-06-09 13:05:48
- **Status:** Correct
- **Marks:** 1

```python
class Solution {
  public:
    void printHollowRect(int n, int m) {
        // code here
    for(int i=1;i<=n;i++){
        for(int j=1;j<=m;j++){
            if(i==1||i==n||j==1||j==m){
                cout<<"*";
            }
            else{
                cout<<" ";
            }
        }
        cout<<"\n";
      }   
    }
};
```

*Generated on: 9/28/2026, 12:44:35 AM*