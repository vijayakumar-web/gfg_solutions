## 01. Remove Spaces

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/remove-spaces0128/1)

### Problem Description

**Task:** Given a string s, remove all the spaces from the string and return the modified string.

#### Examples

##### Example 1

- **Input:**
```text
s = "g eeks for ge eks"Output: "geeksforgeeks"
```
- **Explanation:** All space characters are removed from the given string while preserving the order of the remaining characters, resulting in the final string "geeksforgeeks".

##### Example 2

- **Input:**
```text
s = "abc d "Output: "abcd"
```
- **Explanation:** All space characters are removed from the given string while preserving the order of the remaining characters, resulting in the final string "abcd".

#### Constraints

- **1.** `1 ≤ |s| ≤ 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-18 21:24:45
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public String removeSpaces(String s) {
        String result="";
        for(int i=0;i<s.length();i++)
        {
            if(s.charAt(i)!=' ')
            {
                result=result+s.charAt(i);
            }
        }
        return result;
    }
}
```

*Generated on: 18/11/2026, 9:25:00 pm*