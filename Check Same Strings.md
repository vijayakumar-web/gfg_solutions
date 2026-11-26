## 01. Check Same Strings

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/check-if-two-strings-are-same-or-not--155406/1)

### Problem Description

**Task:** Given two strings s1 and s2, determine if they are exactly the same, considering case sensitivity.Examples:Input: s1 = "abc" , s2 = "abc" Output: trueInput: s1 = " " , s2 = " "Output: trueInput: s1 = "geeks", s2 = "Geeks"Output: false

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-26 10:07:50
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public static boolean areStringsSame(String s1, String s2) {
     return s1.equals(s2);
}
}
```

*Generated on: 26/11/2026, 10:07:59 am*