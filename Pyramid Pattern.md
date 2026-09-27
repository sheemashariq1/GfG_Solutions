## 01. Pyramid Pattern

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/pyramid-patterns/1)

### Problem Description

**Task:** Given a number n, print pyramid pattern with n lines.

#### Examples

##### Example 1

- **Input:**
```text
n = 4 Output: * *** ***** *******
```

##### Example 2

- **Input:**
```text
n = 5 Output: * *** ***** ****************
```

#### Constraints

- **1.** `1 ≤ n ≤ 100`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (3)

#### Solution 1 (Python)

- **Submitted:** 2026-06-13 08:31:11
- **Status:** Correct
- **Marks:** 0

```python
n = int(input())
# code here
for i in range(n):
    for j in range(n-1-i):
        print(" ",end="")
    for j in range(2*i+1):
        print("*",end="")
    print()
```

#### Solution 2 (Python)

- **Submitted:** 2026-06-13 08:26:54
- **Status:** Correct
- **Marks:** 0

```python
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    // code here
    for(int i=0;i<n;i++){
        for(int j=0;j<n-1-i;j++){
            cout<<" ";
        }
        for(int j=0;j<2*i+1;j++){
            cout<<"*";
        }
        cout<<"\n";
    }
    return 0;
}
```

#### Solution 3 (Python)

- **Submitted:** 2026-06-09 11:40:03
- **Status:** Correct
- **Marks:** 1

```python
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;

    // code here
    for (int i = 1; i <= n; i++) {
            for (int j = i; j < n; j++) {
                cout << " ";
            }
            for (int j = 1; j <= (2 * i - 1); j++) {
                cout << "*";
            }
            cout << "\n";
        }
    return 0;
}
```

*Generated on: 9/28/2026, 12:46:46 AM*