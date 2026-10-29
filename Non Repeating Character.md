## 01. Non Repeating Character

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/non-repeating-character-1587115620/1?utm_source=chatgpt.com)

### Problem Description

**Task:** Given a string s consisting of lowercase English Letters. return the first non-repeating character in s. If there is no non-repeating character, return '$'.Examples:Input: s = "geeksforgeeks"

#### Examples

##### Example 1

- **Output:**
```text
'f'
```
- **Explanation:** In the given string, 'f' is the first character in the string which does not repeat.Input: s = "racecar"Output: 'e'Explanation: In the given string, 'e' is the only character in the string which does not repeat.Input: s = "aabbccc"Output: '$'Explanation: All the characters in the given string are repeating.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-29 12:03:03
- **Status:** Correct
- **Marks:** 2

```java
import java.util.HashMap;
class Solution {
    public char nonRepeatingChar(String s) {
        // code here 
        char[] ch = s.toCharArray();
        HashMap<Character, Integer> map = new HashMap<>();
        for (int i = 0; i < s.length(); i++) {
            if (map.containsKey(ch[i])) {
                map.put(ch[i], map.get(ch[i]) + 1);
            } else {
                map.put(ch[i], 1);
            }
        }

        boolean found = false;

        for (int i = 0; i < s.length(); i++) {
            if (map.get(ch[i]) == 1) {
                return ch[i];
            }
        }
        return '$';
    }
}
```

*Generated on: 29/10/2026, 12:03:16 pm*