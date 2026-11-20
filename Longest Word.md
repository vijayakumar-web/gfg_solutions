## 01. Longest Word

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/display-longest-name0853/1)

### Problem Description

**Task:** Given an array arr[] containing strings of names. Your task is to return the longest string. If there are multiple names of the longest size, return the first occurring name.Examples :Input: arr[] = ["Geek", "Geeks", "Geeksfor", "GeeksforGeek", "GeeksforGeeks"]

#### Examples

##### Example 1

- **Output:**
```text
"GeeksforGeeks"Explanation: Name "GeeksforGeeks" has maximum length among all names. Input: arr[] = ["Apple", "Mango", "Orange", "Banana"]Output: "Orange"Explanation: Names "Orange" and "Banana" both have maximum length among all names but Orange comes first so answer will be "Orange".
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-20 19:57:31
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public String longest(String[] arr) {
        int max=0;
        String ans="";
        for(int i=0;i<arr.length;i++)
        {
            if(arr[i].length()>max)
            {
                max=arr[i].length();
                ans=arr[i];
            }
        }
        return ans;
        // code here
        
    }
}
```

*Generated on: 20/11/2026, 7:58:38 pm*