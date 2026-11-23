## 01. Capitalize First Letter of Words

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/upper-case-conversion5419/1)

### Problem Description

**Task:** Given a string s, convert the first letter of each word in the string to uppercase.

#### Examples

##### Example 1

- **Input:**
```text
s = "gEEKs"
```
- **Output:**
```text
"GEEKs"
```

##### Example 2

- **Input:**
```text
s = "i love programming"
```
- **Output:**
```text
"I Love Programming"
```

#### Constraints

- **1.** `1 <= s.length() <= 10⁴Consists of lowercase alphabets and spaces to separate words`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-23 12:25:46
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public String convert(String s) {
        StringBuilder sb=new StringBuilder(s);
        for(int i=0;i<s.length();i++)
        {
            if(i==0||s.charAt(i-1)==' ')
            {
                sb.setCharAt(i, Character.toUpperCase(s.charAt(i)));
            }
        }
                return sb.toString();
    }
}
```

*Generated on: 23/11/2026, 12:26:00 pm*