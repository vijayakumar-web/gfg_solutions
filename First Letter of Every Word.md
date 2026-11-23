## 01. First Letter of Every Word

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/print-first-letter-of-every-word-in-the-string3632/1)

### Problem Description

**Task:** Given a string s, the task is to create a string with the first letter of every word in the string. The string s contains lower case English alphabets and its words have a single space between them.

#### Examples

##### Example 1

- **Input:**
```text
s = "geeks for geeks"
```
- **Output:**
```text
gfgExplanation: First word starts at index 0, take 'g' After first space, next word starts with 'f'After second space, next word starts with 'g'
```

##### Example 2

- **Input:**
```text
s = "bad is good"
```
- **Output:**
```text
big
```

#### Constraints

- **1.** `1 ≤ |s| ≤ 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(|S|)
- **Expected Auxiliary Space Complexity:** O(|S|)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-23 12:33:14
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    String firstAlphabet(String s) {
        StringBuilder sb=new StringBuilder();
        for(int i=0;i<s.length();i++)
        {
            if(i==0||s.charAt(i-1)==' ')
            {
                sb.append(s.charAt(i));
            }
        }
        return sb.toString();
    }
  
}
```

*Generated on: 23/11/2026, 12:33:26 pm*