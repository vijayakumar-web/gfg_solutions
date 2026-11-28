## 01. Decrement Array Values by 1

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/decrement-array-values/1?selectedLang=java)

### Problem Description

**Task:** Given an array arr[] that contains integers. You need to decrement each element of the array by 1 and return the array.Examples:Input: arr[] = [54, 43, 2, 1, 5]

#### Examples

##### Example 1

- **Output:**
```text
323 4 1 1
```
- **Explanation:** Just decrement the numbers by 1.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-28 11:48:05
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public static int[] decrementArray(int[] arr, int n) {
        // code here
     for(int i=0;i<arr.length;i++)
     {
         arr[i]=arr[i]-1;
     }
     return arr;
    }
}
```

*Generated on: 28/11/2026, 11:48:20 am*