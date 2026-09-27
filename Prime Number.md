## 01. Prime Number

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/prime-number2314/1)

### Problem Description

**Task:** Given a number n, determine whether it is a prime number or not.Note: A prime number is a number greater than 1 that has no positive divisors other than 1 and itself.Examples :Input: n = 7

#### Examples

##### Example 1

- **Output:**
```text
false
```
- **Explanation:** 1 has only one divisor (1 itself), which is not sufficient for it to be considered prime.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(sqrt(n))
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (C++)

- **Submitted:** 2026-06-14 11:47:09
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution {
  public:
    bool isPrime(int n) {
        // code here
        if(n<=1){
            return false;
        }
        for(int i=2;i<=n/2;i++){
            if (n%i==0)
            {
                return false;
            }
        }
        return true;
    }
};
```

#### Solution 2 (C++)

- **Submitted:** 2026-06-10 11:03:16
- **Status:** Correct
- **Marks:** 2

```cpp
class Solution {
  public:
    bool isPrime(int n) {
        // code here
        if(n<=1){
            return false;
        }
        for(int i=2;i*i<=n;i++){
            if(n%i==0){
                return false;
            }
        }
        return true;
    }
};
```

*Generated on: 9/28/2026, 12:53:27 AM*