## 01. Check Perfect Square

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/check-perfect-square5253/1)

### Problem Description

**Task:** Given a positive integer n, return true if it is a perfect square, otherwise return false. A number is called a perfect square if it can be written in the form a × a, where a is an integer.

#### Examples

##### Example 1

- **Input:**
```text
n = 35
```
- **Output:**
```text
false
```
- **Explanation:** 35 is not a perfect square.

##### Example 2

- **Input:**
```text
n = 49
```
- **Output:**
```text
true
```
- **Explanation:** 49 is a perfect square (7 * 7 = 49).

#### Constraints

- **1.** `1 ≤ n ≤ 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-24 10:32:44
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public boolean isPerfectSquare(int n) {
        for(long i=0;i*i<=n;i++)
        {
            if(i*i==n)
            {
                return true;
            }
        }
        return false;
        // code here
        
    }
}
```

*Generated on: 24/11/2026, 10:33:44 am*