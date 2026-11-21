## 01. Palindrome Digit Sum

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/sum-of-digit-is-pallindrome-or-not2751/1)

### Problem Description

**Task:** Given a number n. Return true if the digit sum(or sum of digits) of n is a Palindrome number otherwise false.A Palindrome number is a number that stays the same when reversed

#### Examples

##### Example 1

- **Input:**
```text
n = 56
```
- **Output:**
```text
true
```
- **Explanation:** The digit sum of 56 is 5+6 = 11. Since, 11 is a palindrome number.Thus, answer is true.

##### Example 2

- **Input:**
```text
n = 98
```
- **Output:**
```text
false
```
- **Explanation:** The digit sum of 98 is 9+8 = 17. Since 17 is not a palindrome,thus, answer is false.

#### Constraints

- **1.** `1 ≤ n ≤ 10⁹`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-21 09:38:05
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public boolean isDigitSumPalindrome(int n) {
        int sum = 0;

        // Calculate digit sum
        while(n > 0) {
            sum = sum + (n % 10);
            n = n / 10;
        }

        // Reverse the digit sum
        int temp = sum;
        int rev = 0;

        while(temp > 0) {
            int digit = temp % 10;
            rev = rev * 10 + digit;
            temp = temp / 10;
        }

        // Check palindrome
        return sum == rev;
    }
}
```

*Generated on: 21/11/2026, 9:38:21 am*