## 01. First Digit of Number

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/first-digit-of-a-number/1?utm_source=chatgpt.com)

### Problem Description

**Task:** Given a number n, find the first digit of the number.Examples:Input: n = 123

#### Examples

##### Example 1

- **Output:**
```text
1
```

##### Example 2

- **Input:**
```text
n = 976
```
- **Output:**
```text
9
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-02 10:17:04
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public static int firstDigit(int n) {
        while(n>=10)
        {
            n=n/10;
            
        }
        return n;
        // code here
        
    }
}
```

*Generated on: 2/11/2026, 10:17:28 am*