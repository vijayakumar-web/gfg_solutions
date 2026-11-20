## 01. Even Positioned Characters in a String

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/for-loop-2/1)

### Problem Description

**Task:** Given a string s, return a string containing all characters present at even indices (0, 2, 4, ...). The characters must appear in the same order as in the original string.Examples: Input: s = "Geeks"

#### Examples

##### Example 1

- **Output:**
```text
DcoPeoea
```
- **Explanation:** The characters at even indices are collected in their original order.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-20 12:26:17
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public String getEvenCharacters(String s) {
        // code here
        StringBuilder sb=new StringBuilder();
        for(int i=0;i<s.length();i++)
        {
            if(i%2==0)
            {
                sb.append(s.charAt(i));
            }
        }
        return sb.toString();
        
    }
}
```

*Generated on: 20/11/2026, 12:26:32 pm*