## 01. Recursive Sequence

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/recursive-sequence1611/1)

### Problem Description

**Task:** Given an integer n, compute the value of F(n) where F(n) is defined as: F(n) = (1) + (2×3) + (4×5×6) + (7×8×9×10) + …up to n terms.

> **Note:** As the answer can be very large, return the answer modulo 10⁹+7.

#### Examples

##### Example 1

- **Input:**
```text
n = 5
```
- **Output:**
```text
365527
```
- **Explanation:** F(5) = 1 + 2*3 + 4*5*6 + 7*8*9*10 + 11*12*13*14*15 = 365527.

##### Example 2

- **Input:**
```text
n = 7
```
- **Output:**
```text
6997165Explanation: F(7) = 1 + 2*3 + 4*5*6 + 7*8*9*10 + 11*12*13*14*15 + 16*17*18*19*20*21 + 22*23*24*25*26*27*28 = 6006997207.6006997207 % 10⁹+7 = 6997165
```

#### Constraints

- **1.** `1 ≤ n ≤ 100`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-17 21:16:30
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public int sequence(int n) {
        // code here
        long num=1;
        long sum=0;
        long mod=1000000007;
        for(int i=0;i<n;i++)
        {
            long product=1;
            for(int j=0;j<=i;j++)
            {
                product=(product*num)%mod;
                
                num++;
                
            }
            sum=(sum+product)%mod;
            
        }
        return (int)sum;
        
    }
}
```

*Generated on: 17/11/2026, 9:16:46 pm*