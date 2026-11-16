## 01. Sum of Matrix

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/sum-of-elements-in-a-matrix2000/1)

### Problem Description

**Task:** Given an integer matrix mat[][], compute the sum of all its elements.Examples:Input: mat[][] = [[1, 0, 1], [-8, 9, -2]]

#### Examples

##### Example 1

- **Output:**
```text
0
```
- **Explanation:** The sum of all elements of the matrix is: (1 + 0 + 1 + 0 + 1 + 0 + 1 + 0 + 1 + 0 - 1 - 1 - 1 - 1 - 1) = 0.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n * m)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-16 23:33:18
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public int sumOfMatrix(int[][] mat) {
        // code here
    int sum=0;
    for(int[]row:mat)
    {
        for(int val:row)
        {
            sum+=val;
        }
    }
    return sum;
    }
}
```

*Generated on: 16/11/2026, 11:33:40 pm*