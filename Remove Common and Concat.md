## 01. Remove Common and Concat

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/remove-common-characters-and-concatenate-1587115621/1)

### Problem Description

**Task:** Given two strings, s1 and s2. The task is to remove all characters that are common in both strings and then combine the remaining characters from each string to form a new string.
The characters that are not shared between the two strings should appear in the result in the same order as they appear in their respective original strings.
If no characters are left after removing the common characters, return "-1"

#### Examples

##### Example 1

- **Input:**
```text
s1 = aacdb, s2 = gafd
```
- **Output:**
```text
cbgf
```
- **Explanation:** The common characters of s1 and s2 are: a, d. The uncommon characters of s1 and s2 are c, b, g and f. Thus the modified string with uncommon characters concatenated is cbgf.

##### Example 2

- **Input:**
```text
s1 = abcs, s2 = cxzca
```
- **Output:**
```text
bsxz
```
- **Explanation:** The common characters of s1 and s2 are: a,c. The uncommon characters of s1 and s2 are b,s,x and z. Thus the modified string with uncommon characters concatenated is bsxz.

#### Constraints

- **1.** `1 <= |Length of Strings| <= 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-20 20:26:09
- **Status:** Correct
- **Marks:** 1

```java
import java.util.HashSet;

 class Solution {
     public static String concatenatedString(String s1, String s2) {

         HashSet<Character> set1 = new HashSet<>();
         HashSet<Character> set2 = new HashSet<>();

         for(int i = 0; i < s1.length(); i++)
         {
             set1.add(s1.charAt(i));
         }

         for(int i = 0; i < s2.length(); i++)
         {
             set2.add(s2.charAt(i));
         }

         StringBuilder sb = new StringBuilder();

         for(int i = 0; i < s1.length(); i++)
         {
             if(!set2.contains(s1.charAt(i)))
             {
                 sb.append(s1.charAt(i));
             }
         }

         for(int i = 0; i < s2.length(); i++)
         {
             if(!set1.contains(s2.charAt(i)))
             {
                 sb.append(s2.charAt(i));
             }
         }

         if(sb.length() == 0)
         {
             return "-1";
         }

         return sb.toString();
     }
 }
```

*Generated on: 20/11/2026, 8:26:29 pm*