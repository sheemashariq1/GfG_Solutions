## 01. Minimum time to fulfil all orders

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/minimum-time-to-fulfil-all-orders/1)

### Problem Description

**Task:** Geek is organizing a party at his house. For the party, he needs exactly n donuts for the guests. Geek decides to order the donuts from a nearby restaurant, which has m chefs and each chef has a rank r.A chef with rank r can make 1 donut in the first r minutes, 1 more donut in the next 2r minutes, 1 more donut in the next 3r minutes, and so on.For example, a chef with rank 2, can make one donut in 2 minutes, one more donut in the next 4 minutes, and one more in the next 6 minutes. So, it take 2 + 4 + 6 = 12 minutes to make 3 donuts. A chef can move on to making the next donut only after completing the previous one. All the chefs can work simultaneously.Since, it's time for the party, Geek wants to know the minimum time required in completing n donuts. Return an integer denoting the minimum time.

#### Examples

##### Example 1

- **Input:**
```text
n = 10, rank[] = [1, 2, 3, 4]
```
- **Output:**
```text
12 Chef with rank 1, can make 4 donuts in time 1 + 2 + 3 + 4 = 10 mins Chef with rank 2, can make 3 donuts in time 2 + 4 + 6 = 12 mins Chef with rank 3, can make 2 donuts in time 3 + 6 = 9 mins Chef with rank 4, can make 1 donuts in time = 4 minutes Total donuts = 4 + 3 + 2 + 1 = 10 and total time = 12 minutes.
```

##### Example 2

- **Input:**
```text
n = 8, rank[] = [1, 1, 1, 1, 1, 1, 1, 1]
```
- **Output:**
```text
1
```
- **Explanation:** As all chefs are ranked 1, so each chef can make 1 donuts in 1 min. Total donuts = 1 + 1 + 1 + 1 + 1 + 1 + 1 + 1 = 8 and total time = 1 minute.

#### Constraints

- **1.** `1 ≤ n ≤ 10³¹ ≤ m ≤ 10⁴¹ ≤ rank[i] ≤ 100`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(m * log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-06-22 15:44:06
- **Status:** Correct
- **Marks:** 8

```cpp
class Solution {
  public:
    int minTime(vector<int>& ranks, int n) {
        // code here
        long long low=0;
        long long high=1e14;
        long ans=high;
        while(low<=high){
            long long mid=low+(high-low)/2;
            long long total=0;
            for(int r:ranks){
                long long x=(sqrt(1+8.0*mid/r)-1)/2;
                total+=x;
            }
            if(total>=n){
                ans=mid;
                high=mid-1;
            }
            else{
                low=mid+1;
            }
        }
        return ans;
    }
};
```

*Generated on: 9/28/2026, 12:08:56 AM*