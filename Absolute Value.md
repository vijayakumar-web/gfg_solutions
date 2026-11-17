## 01. Absolute Value

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/absolute-value/1)

### Problem Description

**Task:** You are given an interger n, find the absolute value of the integer n.

#### Examples

##### Example 1

- **Input:**
```text
n = -32
```
- **Output:**
```text
32
```
- **Explanation:** The absolute value of -32 is 32.

##### Example 2

- **Input:**
```text
n = 45
```
- **Output:**
```text
45
```
- **Explanation:** The absolute value of 45 is 45 itself.

#### Constraints

- **1.** `-10⁶ ≤ n ≤ 10⁶`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-17 10:15:01
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public int absolute(int n) {
        if(n<0)
        {
            n=n*-1;
        }
        return n;
    }
}
```

*Generated on: 17/11/2026, 10:15:11 am*