## 01. Day Before n Days

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/days-before-n-days/1)

### Problem Description

**Task:** Given two integers d and n. Where d is the day, out of 7 days of the week, d varies from 0 to 6 as shown below.0 - Sunday1 - Monday2 - Tuesday3 - Wednesday4 - Thursday5 - Friday6 - Saturday
You need to return the index for the day which is n days before the given day d.

#### Examples

##### Example 1

- **Input:**
```text
d = 4, n = 3
```
- **Output:**
```text
1
```
- **Explanation:** 3 days before the 4th is 1.

##### Example 2

- **Input:**
```text
d = 2, n = 19
```
- **Output:**
```text
4
```
- **Explanation:** 19 days before the 2nd is 4.

#### Constraints

- **1.** `0 ≤ d ≤ 60 ≤ n ≤ 10⁹`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-15 12:02:40
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public int nthDay(int d, int n) {
                return (d - (n % 7) + 7) % 7;
            }
        }
        // code here
```

*Generated on: 15/11/2026, 12:02:58 pm*