## 01. Floyd's triangle

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/floyds-triangle1222/1)

### Problem Description

**Task:** Given a number n, print Floyd's triangle with n lines.
Floyd’s Triangle is a pattern of consecutive natural numbers arranged in rows, where the i-th row contains i numbers.

#### Examples

##### Example 1

- **Input:**
```text
n = 4 1 2 3 4 5 6 7 8 9 10
```
- **Explanation:** The triangle has 4 rows. Numbers start from 1 and increase sequentially across rows, and each row i contains i elements.

##### Example 2

- **Input:**
```text
n = 5 Output: 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15
```
- **Explanation:** The triangle has 4 rows, and each row i contains i numbers.

#### Constraints

- **1.** `1 <= n <= 100`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (3)

#### Solution 1 (C++)

- **Submitted:** 2026-06-09 11:34:44
- **Status:** Correct
- **Marks:** 0

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    int n;
    cin >> n;
    // code here
    int num=1;
    for(int i=1;i<=n;i++){
        for(int j=1;j<=i;j++){
            cout<<num<<" ";
            num++;
        }
        cout<<endl;
    }
    return 0;
}
```

#### Solution 2 (C++)

- **Submitted:** 2026-06-08 11:55:06
- **Status:** Correct
- **Marks:** 0

```cpp
using System;

class GfG {
    static void Main() {
        int n = int.Parse(Console.ReadLine());
        // code here
        int num=1;
        for(int i=1;i<=n;i++){
            for(int j=1;j<=i;j++){
                Console.Write(num+ " ");
                num++;
            }
            Console.WriteLine();
        }
    }
}
```

#### Solution 3 (C++)

- **Submitted:** 2026-06-08 11:49:58
- **Status:** Correct
- **Marks:** 0

```cpp
import java.util.Scanner;

class GFG {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        // code here
        int num=1;
        for(int i=1;i<=n;i++){
            for(int j=1;j<=i;j++){
                System.out.print(num+" ");
                num++;
            }
            System.out.println();
        }
    }
}
```

*Generated on: 9/28/2026, 12:49:09 AM*