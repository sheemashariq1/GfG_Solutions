## 01. Butterfly Pattern

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/butterfly-pattern/1)

### Problem Description

**Task:** Given a number n. Print Butterfly Pattern with n lines.

#### Examples

##### Example 1

- **Input:**
```text
n = 4 * * ** ** *** *** ******* *** *** ** ** * *
```

##### Example 2

- **Input:**
```text
n = 5 Output: * * ** ** *** *** **** **** ********* **** **** *** *** ** ** * *
```

#### Constraints

- **1.** `1 ≤ n ≤ 100`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (3)

#### Solution 1 (C++)

- **Submitted:** 2026-06-15 09:34:27
- **Status:** Correct
- **Marks:** 0

```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;

    // code here
    for(int i=1;i<=n-1;i++){
        for(int j=1;j<=i;j++){
            cout<<"*";
        }
        int spaces=2*(n-i)-1;
        for(int j=1;j<=spaces;j++){
            cout<<" ";
        }
        for(int j=1;j<=i;j++){
            cout<<"*";
        }
        cout<<endl;
    }
    for(int j=1;j<=2*n-1;j++){
        cout<<"*";
    }
    cout<<endl;
    int stop=max(1,n-95);
    for(int i=n-1;i>=1;i--){
        for(int j=1;j<=i;j++){
            cout<<"*";
        }
        int spaces=2*(n-i)-1;
        for(int j=1;j<=spaces;j++){
            cout<<" ";
        }
        for(int j=1;j<=i;j++){
            cout<<"*";
        }

        cout<<endl;
    }
    return 0;
}
```

#### Solution 2 (C++)

- **Submitted:** 2026-06-09 16:01:10
- **Status:** Correct
- **Marks:** 0

```cpp
n = int(input())
def main():

    # Variables to store number of spaces and stars
    spaces = 2 * n - 1
    stars = 0

    # The outer loop will run for (2 * n - 1) times
    for i in range(1, 2 * n):
        if i <= n:
            spaces = spaces - 2
            stars += 1

        # Lower half of the butterfly
        else:
            spaces = spaces + 2
            stars -= 1

        # Print stars
        for j in range(1, stars + 1):
            print("*", end="")

        # Print spaces
        for j in range(1, spaces + 1):
            print(" ", end="")

        # Print stars
        for j in range(1, stars + 1):
            if j != n:
                print("*", end="")

        print()
main()
```

#### Solution 3 (C++)

- **Submitted:** 2026-06-09 15:54:45
- **Status:** Correct
- **Marks:** 0

```cpp
# code here
def main():
    import sys
    # Using sys.stdin.read split handles fast I/O for large inputs like n = 100
    input_data = sys.stdin.read().split()
    if not input_data:
        return
    n = int(input_data[0])
    
    output = []
    # 1. Upper Half (Rows 1 to n-1)
    for i in range(1, n):
        stars = "*" * i
        # Total line width is 2n - 1. 
        # Spaces = (2n - 1) - (2 * stars)
        spaces = " " * ((2 * n - 1) - (2 * i))
        output.append(stars + spaces + stars)
        
    # 2. Middle Row (Row n)
    # The middle row has no spaces and exactly 2n - 1 stars
    output.append("*" * (2 * n - 1))
    
    # 3. Lower Half (Rows n-1 down to 1)
    for i in range(n - 1, 0, -1):
        stars = "*" * i
        spaces = " " * ((2 * n - 1) - (2 * i))
        output.append(stars + spaces + stars)
        
    # Join everything with newlines and print all at once for maximum speed
    print("\n".join(output))
if __name__ == "__main__":
    main()
```

*Generated on: 9/28/2026, 12:43:41 AM*