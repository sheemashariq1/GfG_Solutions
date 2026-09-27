## 01. URLify a given string

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/urlify-a-given-string--141625/1)

### Problem Description

**Task:** Given a string s, replace all the spaces in the string with '%20'.Examples:Input: s = "i love programming"Output: "i%20love%20programming"

#### Examples

##### Example 1

- **Output:**
```text
"Mr%20Benedict%20Cumberbatch"
```
- **Explanation:** The 2 spaces are replaced by '%20'

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-18 12:37:29
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    string URLify(string &s) {
        // code here
        string result="";
        for(char c:s){
            if(c==' '){
                result+="%20";
            }
            else{
                result+=c;
            }
        }
        return result;
    }
};
```

*Generated on: 9/28/2026, 12:37:36 AM*