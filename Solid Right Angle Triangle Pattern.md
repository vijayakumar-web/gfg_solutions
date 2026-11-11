## 01. Solid Right Angle Triangle Pattern

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/right-angle-triangle-1605685807/1)

### Problem Description

**Task:** Given an integer n. Write a program to print the Right angle triangle wall. The length of perpendicular and base is s. Note: Print exactly single " " after "*". Print a new line after printing the triangle.Examples:Input: n = 4

#### Examples

##### Example 1

- **Explanation:** * * * * * * * * * * Explanation: Length of perpendicular and base of triangle is 4 .Input: n = 3 * * * * * * Explanation: Length of perpendicular and base of triangle is 3.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-11 21:41:23
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public void printPattern(int n) {
        // code here
        for(int i=0;i<n;i++)
        {
            for(int j=0;j<=i;j++)
            {
                if(j<=i)
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

*Generated on: 11/11/2026, 9:41:38 pm*