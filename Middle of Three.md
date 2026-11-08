## 01. Middle of Three

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/middle-of-three2926/1)

### Problem Description

**Task:** Given three distinct numbers a, b and c. Find the number with a value in the middle (Try to do it with minimum comparisons).

#### Examples

##### Example 1

- **Input:**
```text
a = 978, b = 518, c = 300
```
- **Output:**
```text
518
```
- **Explanation:** Since 518 > 300 and 518 < 978, so 518 is the middle element.

##### Example 2

- **Input:**
```text
a = 162, b = 934, c = 200
```
- **Output:**
```text
200 Exaplanation: Since 200 > 162 && 200 < 934, So, 200 is the middle element.
```

##### Example 3

- **Input:**
```text
a = 246, b = 214, c = 450
```
- **Output:**
```text
246
```

#### Constraints

- **1.** `1 <= a, b, c <= 10⁹a, b, c are distinct.`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-08 23:43:58
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    int middle(int a, int b, int c) {
        if((a>b&&a<c)||(a<b&&a>c))
        {
            return a;
        }
        else if((b<a&&b>c)||(b>a&&b<c))
        {
            return b;
        }
        else
        {
            return c;
        }
    }
}
```

*Generated on: 8/11/2026, 11:44:38 pm*