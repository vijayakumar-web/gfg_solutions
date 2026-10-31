## 01. Print Hollow Square

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/print-square--105330/1)

### Problem Description

**Task:** Given an integer n, print the hollow square pattern of size n using '*' character. Examples:Input: n = 4

#### Examples

##### Example 1

- **Explanation:** It's a hollow square! Each side contains n = 4.Input: n = 3 * * * * ** * *Explanation: It's a hollow square! Each side contains n = 3.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-31 20:37:06
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public void printHollowSquare(int n) {
        for(int i=0;i<n;i++)
        {
            for(int j=0;j<n;j++)
            {
                if(i==0||i==n-1||j==0||j==n-1)
                {
                    System.out.print("* ");
                }
                else
                {
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}
```

*Generated on: 31/10/2026, 8:37:23 pm*