## 01. Convert Celsius To Fahrenheit

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/convert-celsius-to-fahrenheit/1)

### Problem Description

**Task:** Given a temperature in celsius c. You need to convert the given temperature into Fahrenheit.Note: The driver code handles precision and prints the result rounded up to 2 decimal places.Examples:Input: c = 32

#### Examples

##### Example 1

- **Output:**
```text
122
```
- **Explanation:** Using the conversion formula of celsius to farhenheit, it can be calculated that, for 50 degree C, the temperature in Fahrenheit = 122.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-17 10:11:25
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
     public double cToF(int C) {
         double F = (C * 9.0 / 5.0) + 32;
         return F;
     }
 }
```

*Generated on: 17/11/2026, 10:11:34 am*