## 01. Factorial

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/factorial5739/1)

### Problem Description

**Task:** Given a positive integer, n. Find the factorial of n.Examples :Input: n = 5

#### Examples

##### Example 1

- **Output:**
```text
24
```
- **Explanation:** 1 x 2 x 3 x 4 = 24

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (5)

#### Solution 1 (C++)

- **Submitted:** 2026-06-29 10:06:27
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution {
  public:
    int factorial(int n) {
        // code here
        int fact=1;
        for(int i=1;i<=n;i++){
            fact*=i;
        }
        return fact;
    }
};
```

#### Solution 2 (C++)

- **Submitted:** 2026-06-11 11:51:27
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution:
    # Function to calculate factorial of a number.
    def factorial(self, n: int) -> int:
        # code here
        fact=1
        for i in range(1,n+1):
            fact=fact*i
            
        return (fact)
```

#### Solution 3 (C++)

- **Submitted:** 2026-06-11 11:49:19
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution {
  public:
    int factorial(int n) {
        // code here
        int fact=1;
        for(int i=1;i<=n;i++){
            fact*=i;
        }
        return fact;
    }
};
```

#### Solution 4 (C++)

- **Submitted:** 2026-06-11 11:49:01
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution {
  public:
    int factorial(int n) {
        // code here
        int fact=1;
        for(int i=1;i<=n;i++){
            fact*=i;
        }
        return fact;
    }
};
```

#### Solution 5 (C++)

- **Submitted:** 2026-06-08 11:33:11
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    int factorial(int n) {
        // code here
        int res=1;
        for(int i=1;i<=n;i++){
            res=res*i;
        }
        return res;
    }
};
```

*Generated on: 9/28/2026, 12:49:57 AM*