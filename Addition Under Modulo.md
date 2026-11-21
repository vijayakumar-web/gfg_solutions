## 01. Addition Under Modulo

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/addition-under-modulo/1)

### Problem Description

**Task:** Given three integers a, b, and M, compute the result of the modular addition operation: (a+b) mod M

> **Note:** Modular operations returns the remainder when divided by M. The result will always lie in the range 0 and M - 1.

#### Examples

##### Example 1

- **Input:**
```text
a = 10, b = 20, M = 3
```
- **Output:**
```text
0
```
- **Explanation:** (10 + 20) mod 3 = 0

##### Example 2

- **Input:**
```text
a = 100, b = 13, M = 107
```
- **Output:**
```text
6
```
- **Explanation:** (100 + 13) mod 107 = 6

#### Constraints

- **1.** `1 ≤ a, b , M ≤ 10⁹`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-21 11:04:08
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public int sumUnderModulo(int a, int b, int M) {
      return (int)(long)(a+b)%M;
    }
}
```

*Generated on: 21/11/2026, 11:04:21 am*