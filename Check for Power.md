## 01. Check for Power

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/check-if-a-number-is-power-of-another-number5442/1)

### Problem Description

**Task:** Given two positive integers x and y, determine if y is a power of x. If y is a power of x, return true. Otherwise, return false.

#### Examples

##### Example 1

- **Input:**
```text
x = 2, y = 8
```
- **Output:**
```text
true Explanation: 2³ is equal to 8.
```

##### Example 2

- **Input:**
```text
x = 1, y = 8
```
- **Output:**
```text
false
```
- **Explanation:** Any power of 1 is not equal to 8.

##### Example 3

- **Input:**
```text
x = 46, y = 205962976
```
- **Output:**
```text
true
```
- **Explanation:** 46⁵ is equal to 205962976.

##### Example 4

- **Input:**
```text
x = 50, y = 312500000
```
- **Output:**
```text
true
```
- **Explanation:** 50⁵ is equal to 312500000.

#### Constraints

- **1.** `1 ≤ x ≤ 10³¹ ≤ y ≤ 10⁹`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-09 12:31:10
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public boolean isPower(int x, int y) {
        if(x==1)
        {
            return y==1;
        }
        while(y>1)
        {
        if(y%x!=0)
        {
            return false;
        }
            y=y/x;
        }
        return true;
    }
}
```

*Generated on: 9/11/2026, 12:31:25 pm*