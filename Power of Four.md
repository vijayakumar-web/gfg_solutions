## 01. Power of Four

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/power-of-four/1)

### Problem Description

**Task:** Given a number n, check if n is power of 4 or not.

#### Examples

##### Example 1

- **Input:**
```text
n = 64
```
- **Output:**
```text
true
```
- **Explanation:** 4³ = 64

##### Example 2

- **Input:**
```text
n = 75
```
- **Output:**
```text
false
```
- **Explanation:** 75 is not a power of 4.

#### Constraints

- **1.** `1 ≤ n ≤ 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-24 10:36:57
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    boolean isPowerOfFour(int n) {
        while(n>0 && n%4==0)
        {
            n=n/4;
        }
        return n==1;
        // code here
        
    }
}
```

*Generated on: 24/11/2026, 10:37:05 am*