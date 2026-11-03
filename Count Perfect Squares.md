## 01. Count Perfect Squares

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/count-squares3649/1)

### Problem Description

**Task:** Given a positive integer n, find the number of perfect squares that are less than n in the sample space of perfect squares. The sample space consists of all perfect squares starting from 1 (i.e., 1, 4, 9, 16, 25, …)Examples :Input: n = 9

#### Examples

##### Example 1

- **Output:**
```text
1
```
- **Explanation:** 1 is the only Perfect Square less than 3. So, the Output is 1.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** sqrt(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-03 20:56:52
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    static int countSquares(int n) {
        int count = 0;

        for (int i = 1; i * i < n; i++) {
            count++;
        }

        return count;
    }
}
```

*Generated on: 3/11/2026, 8:57:05 pm*