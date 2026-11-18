## 01. Remove Vowels

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/remove-vowels-from-string1446/1)

### Problem Description

**Task:** Given a string s. Your task is to remove the vowels from the string.

#### Examples

##### Example 1

- **Input:**
```text
s = "welcome to geeksforgeeks"
```
- **Output:**
```text
"wlcm t gksfrgks"
```
- **Explanation:** Vowels were ignored only consonents were returned in the same order.

##### Example 2

- **Input:**
```text
s = "what is your name ?"
```
- **Output:**
```text
wht s yr nm ?
```

#### Constraints

- **1.** `1 <= |s| <= 10⁵Alphabets are lower cases only`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-18 23:08:05
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
     String removeVowels(String s) {
         StringBuilder result = new StringBuilder();

         for(int i = 0; i < s.length(); i++) {
             char ch = s.charAt(i);

             if(ch != 'a' && ch != 'A' &&
                ch != 'e' && ch != 'E' &&
                ch != 'i' && ch != 'I' &&
                ch != 'o' && ch != 'O' &&
                ch != 'u' && ch != 'U') {

                 result.append(ch);
             }
         }

         return result.toString();
     }
 }
```

*Generated on: 18/11/2026, 11:08:27 pm*