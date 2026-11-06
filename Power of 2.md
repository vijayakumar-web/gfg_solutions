## 01. Power of 2

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/power-of-2-1587115620/1)

### Problem Description

**Task:** Given a non-negative integer n, return true if it is a power of 2. Otherwise, return false. Examples:Input: n = 8

#### Examples

##### Example 1

- **Output:**
```text
true
```
- **Explanation:** 1 is equal to 2 raised to 0 (2⁰ = 1).

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-06 12:00:09
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public boolean isPowerofTwo(int n) {
        if(n==1)
        {
            return true;
        }
        if(n<=0)
        {
            return false;
        }
        while(n%2==0)
        {
            
            n=n/2;
        }
        return n==1;
    }
}
```

*Generated on: 6/11/2026, 12:00:24 pm*