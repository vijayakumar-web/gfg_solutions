## 01. Check Arithmetic Progression

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/check-arithmetic-progression1842/1)

### Problem Description

**Task:** Given an array arr[] of integers. Write a program to check whether an arithmetic progression can be formed using all the given elements. Examples:Input: arr[] = [0, 12, 4, 8]

#### Examples

##### Example 1

- **Output:**
```text
falseExplanation: there is no rearrangment which can forms an arithmetic progression.
```
- **Explanation:** Rearrange given array as [0, 4, 8, 12] which forms an arithmetic progression.Input: arr[] = [12, 40, 11, 20]

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-19 21:18:33
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    // Function to check if the given array forms an arithmetic progression
    public boolean checkIsAP(int[] arr) {
        // Your code goes here
        Arrays.sort(arr);
        int diff=arr[1]-arr[0];
        for(int i=2;i<arr.length;i++)
        {
            if(arr[i]-arr[i-1]!=diff)
            {
                return false;
            }
        }
        return true;
        
    }
}
```

*Generated on: 19/11/2026, 9:18:46 pm*