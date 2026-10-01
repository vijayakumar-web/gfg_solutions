## 01. Ways to Reach Origin

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/paths-to-reach-origin3850/1)

### Problem Description

**Task:** Geek is standing at a point (x, y) on a 2D grid and wants to reach the origin (0, 0). From any point, Geek can move in only two directions: left, from (x, y) to (x - 1, y), or down, from (x, y) to (x, y - 1).Find the total number of distinct paths for Geek to reach (0, 0) from (x, y). Since the answer can be very large, return it modulo 10⁹+7.Examples:Input: x = 3, y = 0

#### Examples

##### Example 1

- **Output:**
```text
84
```
- **Explanation:** There are a total of 84 distinct paths from (3, 6) to (0, 0) using only left and down moves.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(x · y)
- **Expected Auxiliary Space Complexity:** O(x · y)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-01 10:56:05
- **Status:** Correct
- **Marks:** 4

```java
class Solution {
    public int ways(int x, int y) {

        int MOD = 1000000007;

        int[] dp = new int[y + 1];

        // First row
        for (int i = 0; i <= y; i++) {
            dp[i] = 1;
        }

        for (int i = 1; i <= x; i++) {

            for (int j = 1; j <= y; j++) {

                dp[j] = (dp[j] + dp[j - 1]) % MOD;
            }
        }

        return dp[y];
    }
}
```

*Generated on: 1/10/2026, 10:56:25 am*