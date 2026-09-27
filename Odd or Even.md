## 01. Odd or Even

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/odd-or-even3618/1)

### Problem Description

**Task:** Given a positive integer n, find if it is odd or even. Return true if the number is even else false.Examples:Input: n = 15

#### Examples

##### Example 1

- **Output:**
```text
false
```
- **Explanation:** The number is not divisible by 2, Odd number.Input: n = 44Output: trueExplanation: The number is divisible by 2, Even number.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (5)

#### Solution 1 (Code)

- **Submitted:** 2026-06-04 12:56:49
- **Status:** Correct
- **Marks:** 0

```csharp
class Solution {
    public bool isEven(int n) {
        // code here
        if (n%2==0)
        return true;
        else
        return false;
    }
}
```

#### Solution 2 (Code)

- **Submitted:** 2026-06-04 12:55:46
- **Status:** Correct
- **Marks:** 0

```csharp
/**
 * @param {number} n
 * @return {bool}
 */

class Solution {
    isEven(n) {
        // code here
        if (n%2==0)
        return true;
        else
        return false;
    }
}
```

#### Solution 3 (Code)

- **Submitted:** 2026-06-04 12:54:37
- **Status:** Correct
- **Marks:** 0

```csharp
#include <stdbool.h>
int isEven(int n) {
    // code here
    if(n%2==0)
    return true;
    else
    return false;
}
```

#### Solution 4 (Code)

- **Submitted:** 2026-06-04 12:49:40
- **Status:** Correct
- **Marks:** 0

```csharp
class Solution:
    def isEven (self, n):
        # code here 
        if n%2==0:
            return True
        else:
            return False
```

#### Solution 5 (Code)

- **Submitted:** 2026-06-04 12:48:32
- **Status:** Correct
- **Marks:** 1

```csharp
class Solution {
  public:
    bool isEven(int n) {
        // code here
        if(n%2==0)
        return true;
        else
        return false;
    }
};
```

*Generated on: 9/28/2026, 12:54:28 AM*