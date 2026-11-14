## 01. Print Hollow Rectangle

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/hollow-rectangle-or-square/1)

### Problem Description

**Task:** Given two integers n and m, print a hollow rectangle pattern consisting of n rows and m columns using '*' character. Examples:Input: n = 3, m = 5Output:****** ******Explanation: It's a hollow rectangle with 3 rows and 5 columns.Input: n = 4, m = 3Output:**** ** * ***Explanation: It's a hollow rectangle with 4 rows and 3 columns.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n * m)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-14 10:23:26
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public void printHollowRect(int n, int m) {
        for(int i=1;i<=n;i++)
        {
            for(int j=1;j<=m;j++)
            {
                if(i==1||j==1||i==n||j==m)
                {
                    System.out.print("*");
                }
                else
                {
                    System.out.print(" ");
                }
            }
            System.out.println();
        }
        // code here
        
    }
}
```

*Generated on: 14/11/2026, 10:23:39 am*