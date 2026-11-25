## 01. Sum of n Even Squares

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/power-of-pow-even-number5440/1)

### Problem Description

**Task:** Given a single integer n, your task is to find the sum of the square of the first n even natural Numbers. Examples:Input: n = 2

#### Examples

##### Example 1

- **Output:**
```text
20
```
- **Explanation:** 2² + 4² = 20

##### Example 2

- **Input:**
```text
n = 3
```
- **Output:**
```text
56
```
- **Explanation:** 2² + 4² + 6² = 56

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-25 23:27:34
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public int sumSqEven(int n) {
      long sum=0;
      for(int i=1;i<=n;i++)
      {
          long even=i*2;
          sum=sum+(even*even);
      }
      return (int)sum;
    }
}
```

*Generated on: 25/11/2026, 11:27:45 pm*