## 01. Count Digits in Number

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/count-total-digits-in-a-number/1?utm_source=chatgpt.com)

### Problem Description

**Task:** Given a number n, return the count of digits in this number.Examples :Input: n = 1567

#### Examples

##### Example 1

- **Output:**
```text
5
```
- **Explanation:** The number of digits in 99999 is 5.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-26 13:59:13
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public int countDigits(int n) {
        int count=0;
        if(n==0)
        {
            return 1;
        }
       while(n>0)
        {
            n=n/10;
            count++;
        }
        return count;
    }
}
```

*Generated on: 26/10/2026, 1:59:27 pm*