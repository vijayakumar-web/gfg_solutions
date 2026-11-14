## 01. Square Root

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/square-root/1)

### Problem Description

**Task:** Given a positive integer n, find the square root of n. If n is not a perfect square, then return the floor value.Floor value of any number is the greatest Integer which is less than or equal to that number.Examples: Input: n = 4

#### Examples

##### Example 1

- **Output:**
```text
1Explanation: 1 is a perfect square, so its square root is 1.
```
- **Explanation:** Since, 11 is not a perfect square, floor of square root of 11 is 3.Input: n = 1

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-15 00:54:35
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    int floorSqrt(int n) {
        int ans=0;
        for(int i=1;i*i<=n;i++)
        {
            if(i*i==n)
            {
            return i;
            }
            ans=i;
        }
        return ans;
        
        // code here
        
    }
}
```

*Generated on: 15/11/2026, 12:54:52 am*