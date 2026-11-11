## 01. Hollow Right Angle Triangle Pattern

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/right-angle-triangle-2-1605689820--102106/1)

### Problem Description

**Task:** Given an integer n. Write a program to print the Right angle triangle. The length of the perpendicular and base is n. Examples : Input: n = 9

#### Examples

##### Example 1

- **Output:**
```text
** ** ** ** ** ** ** ** * * * * * * * *
```
- **Explanation:** Length of perpendicular and base of triangle is 9.Input: n = 4Output:** ** ** * * *Explanation: Length of perpendicular and base of triangle is 4.Constraints:1 ≤ n ≤ 12

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-11 22:26:40
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public void printPattern(int n) {
        for(int i=0;i<n;i++)
        {
            for(int j=0;j<=i;j++)
            {
                if(j==0||j==i||i==n-1)
                {
                    System.out.print("* ");
                }
                else
                {
                    System.out.print("  ");
                }
                // System.out.println();
                
            }
            System.out.println();
        }
        
    }
}
```

*Generated on: 11/11/2026, 10:26:53 pm*