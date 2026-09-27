## 01. Josephus problem

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/josephus-problem/1)

### Problem Description

**Task:** You are playing a game with n people standing in a circle, numbered from 1 to n. Starting from person 1, every k^th person is eliminated in a circular fashion. The process continues until only one person remains.Given integers n and k, return the position (1-based index) of the person who will survive.

#### Examples

##### Example 1

- **Input:**
```text
n = 5, k = 2
```
- **Output:**
```text
3
```
- **Explanation:** Firstly, the person at position 2 is killed, then the person at position 4 is killed, then the person at position 1 is killed. Finally, the person at position 5 is killed. So the person at position 3 survives.

##### Example 2

- **Input:**
```text
n = 7, k = 3
```
- **Output:**
```text
4
```
- **Explanation:** The elimination order is 3 → 6 → 2 → 7 → 5 → 1, and the person at position 4 survives.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (2)

#### Solution 1 (C++)

- **Submitted:** 2026-06-15 09:42:47
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution {
  public:
    int josephus(int n, int k) {
        // code here
        int res=0;
        for(int i=2;i<=n;i++){
            res=(res+k)%i;
    }
    return res+1;
    }
};
```

#### Solution 2 (C++)

- **Submitted:** 2026-06-10 11:11:01
- **Status:** Correct
- **Marks:** 2

```cpp
class Solution {
  public:
    int josephus(int n, int k) {
        // code here
        int sur=0;
        for(int i=2;i<=n;i++){
            sur=(sur+k)%i;
        }
        return sur+1;
    }
};
```

*Generated on: 9/28/2026, 12:12:39 AM*