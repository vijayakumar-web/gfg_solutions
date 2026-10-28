## 01. Corner Digits Sum

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/corner-digits1317/1)

### Problem Description

**Task:** Given a positive integer n, find the sum of the first and the last digit of n. Examples:

#### Examples

##### Example 1

- **Input:**
```text
n = 12345
```
- **Output:**
```text
6
```
- **Explanation:** 1st and last digits are 1 and 5.

##### Example 2

- **Input:**
```text
n = 98562
```
- **Output:**
```text
11
```
- **Explanation:** 1st and last digits are 9 and 2.

#### Constraints

- **1.** `1 ≤ n ≤ 10⁹`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O( log10(n) )
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-28 09:38:38
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public int cornerDigitSum(int n) {
        int last=n%10;
        int first=n;
        while(first >= 10)
        {
            first=first/10;
            
        }
        return first+last;
    }
}
```

*Generated on: 28/10/2026, 9:38:47 am*