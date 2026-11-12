## 01. Elements in Range

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/elements-in-the-range2834/1)

### Problem Description

**Task:** Given an array arr[] containing distinct positive integers, and two integers start and end defining a range. Find if the array contains all elements within inclusive range [start, end].Examples :Input: start = 2, end = 5, arr[] = [1, 4, 5, 2, 7, 8, 3]

#### Examples

##### Example 1

- **Output:**
```text
false
```
- **Explanation:** The array does not contain 6; hence, it does not contain all the elements in the range [2, 6]. Therefore, the output is false.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-12 22:32:26
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public boolean checkElements(int start, int end, int[] arr) {
        // code here
        for(int i=start;i<=end;i++)
        {
            boolean found=false;
            for(int j=0;j<arr.length;j++)
            {
                if(arr[j]==i)
                {
                    found=true;
                    break;
                }
            }
            if(found==false)
            {
                return false;
            }
        }
            return true;
        
        
    }
}
```

*Generated on: 12/11/2026, 10:32:39 pm*