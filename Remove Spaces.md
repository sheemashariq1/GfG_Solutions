## 01. Remove Spaces

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/remove-spaces0128/1)

### Problem Description

**Task:** Given a string s, remove all the spaces from the string and return the modified string.

#### Examples

##### Example 1

- **Input:**
```text
s = "g eeks for ge eks"Output: "geeksforgeeks"
```
- **Explanation:** All space characters are removed from the given string while preserving the order of the remaining characters, resulting in the final string "geeksforgeeks".

##### Example 2

- **Input:**
```text
s = "abc d "Output: "abcd"
```
- **Explanation:** All space characters are removed from the given string while preserving the order of the remaining characters, resulting in the final string "abcd".

#### Constraints

- **1.** `1 ≤ |s| ≤ 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (C++)

- **Submitted:** 2026-06-17 11:32:32
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution {
  public:
    string removeSpaces(string& s) {
        // code here
        int index=0;
        for(int i=0;i<s.length();i++){
            if(s[i]!=' '){
                s[index]=s[i];
                index++;
            }
        }
        s.erase(index);
        return s;
    }
};
```

#### Solution 2 (C++)

- **Submitted:** 2026-06-17 11:32:11
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    string removeSpaces(string& s) {
        // code here
        int index=0;
        for(int i=0;i<s.length();i++){
            if(s[i]!=' '){
                s[index]=s[i];
                index++;
            }
        }
        s.erase(index);
        return s;
    }
};
```

*Generated on: 9/28/2026, 12:38:03 AM*