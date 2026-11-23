## 01. Check Palindrome Ignoring Case

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/check-palindrome--141628/1)

### Problem Description

**Task:** Given a string s consisting only of English alphabets, check whether it is a palindrome or not, ignoring the case of the letters. A string is a palindrome if it reads the same forward and backward when case differences are ignored. Return true if s is a palindrome, otherwise return false.Examples:Input: s = "Hello"

#### Examples

##### Example 1

- **Output:**
```text
true
```
- **Explanation:** TenEt = = tEneT as we are ignoring the case.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-23 12:39:50
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
     public boolean isPalindrome(String s) {
         String org = s.toLowerCase();
         String rev = "";

         for(int i = org.length()-1; i >= 0; i--) {
             rev = rev + org.charAt(i);
         }

         if(rev.equals(org)) {
             return true;
         }

         return false;
     }
 }
```

*Generated on: 23/11/2026, 12:40:03 pm*