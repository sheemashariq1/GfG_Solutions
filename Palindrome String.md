## 01. Palindrome String

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/palindrome-string0817/1)

### Problem Description

**Task:** Given a string s, find if it is a palindrome. A string is considered a palindrome if it reads the same forwards and backwards.

#### Examples

##### Example 1

- **Input:**
```text
s = "abba"
```
- **Output:**
```text
true
```
- **Explanation:** "abba" reads the same forwards and backwards, so it is a palindrome.

##### Example 2

- **Input:**
```text
s = "abc"
```
- **Output:**
```text
false
```
- **Explanation:** "abc" does not read the same forwards and backwards, so it is not a palindrome.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-17 11:24:25
- **Status:** Correct
- **Marks:** 2

```cpp
class Solution {
  public:
    bool isPalindrome(string& s) {
        // code here
        int left=0;
        int right=s.length()-1;
        while(left<right){
            if(s[left]!=s[right]){
                return false;
            }
            left++;
            right--;
        }
        return true;
    }
};
```

*Generated on: 9/28/2026, 12:39:16 AM*