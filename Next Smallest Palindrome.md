## 01. Next Smallest Palindrome

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/next-smallest-palindrome4740/1)

### Problem Description

**Task:** Given a number, in the form of an array arr[] containing digits from 1 to 9(inclusive). Find the next smallest palindrome strictly larger than the given number.

#### Examples

##### Example 1

- **Input:**
```text
arr[] = [9, 4, 1, 8, 7, 9, 7, 8, 3, 2, 2]
```
- **Output:**
```text
[9, 4, 1, 8, 8, 0, 8, 8, 1, 4, 9]
```
- **Explanation:** Next smallest palindrome is 9 4 1 8 8 0 8 8 1 4 9.

##### Example 2

- **Input:**
```text
arr[] = [2, 3, 5, 4, 5]
```
- **Output:**
```text
[2, 3, 6, 3, 2]
```
- **Explanation:** Next smallest palindrome is 2 3 6 3 2.

#### Constraints

- **1.** `1 ≤ n ≤ 10⁵¹ ≤ arr[i] ≤ 9`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-20 11:33:13
- **Status:** Correct
- **Marks:** 8

```cpp
class Solution {
  public:
    vector<int> nextPalindrome(vector<int>& num) {
        // code here
        int n=num.size();
        bool all=true;
        for(int x:num){
            if(x!=9){
                all=false;
                break;
            }
        }
        if(all){
            vector<int> ans(n+1,0);
            ans[0]=1;
            ans[n]=1;
            return ans;
        }
        int mid=n/2;
        int i=mid-1;
        int j=(n%2==0)?mid:mid+1;
        while(i>=0 && num[i]==num[j]){
            i--;
            j++;
        }
        bool incre=false;
        if(i<0 || num[i] < num[j]){
            incre=true;
        }
        i=mid-1;
        j=(n%2==0)?mid:mid+1;
        while(i>=0){
            num[j]=num[i];
            i--;
            j++;
        }
        if(incre){
            int carry=1;
            if(n%2==1){
                num[mid]+=carry;
                carry=num[mid]/10;
                num[mid]%=10;
                i=mid-1;
                j=mid+1;
            }
            else{
                i=mid-1;
                j=mid;
            }
            while(i>=0){
                num[i]+=carry;
                carry=num[i]/10;
                num[i]%=10;
                num[j]=num[i];
                i--;
                j++;
            }
        }
        return num;
    }
};
```

*Generated on: 9/28/2026, 12:11:15 AM*