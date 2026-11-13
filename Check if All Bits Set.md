## 01. Check if All Bits Set

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/check-set-bits5408/1)

### Problem Description

**Task:** Given a number n, check whether every bit in the binary representation of the given number is set or not.
Return true if yes, otherwise false.

#### Examples

##### Example 1

- **Input:**
```text
n = 7
```
- **Output:**
```text
true
```
- **Explanation:** Binary for 7 is 111 all the bits are set so the output is true.

##### Example 2

- **Input:**
```text
n = 8
```
- **Output:**
```text
false
```
- **Explanation:** Binary for 8 is 1000 all the bits are not set so the output is false.

##### Example 3

- **Input:**
```text
n = 0
```
- **Output:**
```text
false
```
- **Explanation:** All the bits are 0 so the output is false.

#### Constraints

- **1.** `0 ≤ n ≤ 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-13 10:47:33
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public boolean isBitSet(int n) {
        // code here
        if(n==0)
        {
            return false;
        }
        while(n>0)
        {
            if((n&1)==0)
            {
                return false;
            }
            n=n>>1;
        }
        return true;
    }
}
```

*Generated on: 13/11/2026, 10:47:45 am*