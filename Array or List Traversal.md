## 01. Array or List Traversal

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/array-traversal/1)

### Problem Description

**Task:** Given an array arr[] that contains integers. Print the elements of the array in a single line with a space between them.Note: Don't add a new line at the end.Examples:Input: arr[] = [54, 43, 2, 1, 5]

#### Examples

##### Example 1

- **Output:**
```text
324 5 2 2
```
- **Explanation:** Just traverse and print the numbers.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-08-08 12:25:49
- **Status:** Correct
- **Marks:** 1

```cpp
void arrayTraversal(int numbers[], int size) {
    // Code here
    for (int i=0;i<size;i++){
        cout<<numbers[i]<<" ";
    }
}
```

*Generated on: 9/28/2026, 12:26:31 AM*