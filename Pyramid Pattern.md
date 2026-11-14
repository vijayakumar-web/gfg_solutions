## 01. Pyramid Pattern

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/pyramid-patterns/1)

### Problem Description

**Task:** Given an integer n, print a pyramid pattern of stars with n rows. Each row consists of leading spaces followed by asterisks such that the stars are centered, with the first row having 1 star and each subsequent row having 2 more stars than the previous row.Examples:Input: n = 4 Output: * *** ************Explanation: The pyramid has 4 rows. Row 1 has 3 leading spaces and 1 star, row 2 has 2 leading spaces and 3 stars, row 3 has 1 leading space and 5 stars, and row 4 has 0 leading spaces and 7 stars.Input: n = 5 Output: * *** ***** ****************Explanation: The pyramid has 1 row with 0 leading spaces and 1 star.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-14 10:38:07
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public void printPyramid(int n) {
        // code here
        for(int i=1;i<=n;i++)
        {
            for(int j=1;j<=n-i;j++){
                System.out.print(" ");
            }
            for(int j=1; j<=2*i-1; j++)
            {
                System.out.print("*");
            }

            System.out.println();
        }
        
    }
}
```

*Generated on: 14/11/2026, 10:38:19 am*