## 01. Mean or Average of Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/mean0021/1)

### Problem Description

**Task:** Given an array arr[], return the floor value of the mean of its elements.Examples:Input: arr[] = [1, 3, 4, 2, 6, 5, 8, 7]Output: 4Explanation: Sum of the elements is 1 + 3 + 4 + 2 + 6 + 5 + 8 + 7 = 36, Mean = 36/8 = 4.5, floor(4.5) = 4.Input: arr[] = [4, 4, 4, 4, 4]Output: 4Explanation: Sum of the elements is 4 + 4 + 4 + 4 + 4 = 20, Mean = 20/5 = 4

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-02 17:49:13
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public static int findMean(int[] arr) {
        int sum=0;
        int n=arr.length;
        for(int i=0;i<arr.length;i++)
        {
            sum=sum+arr[i];
        }
        return sum/n;
        // code here
        
    }
};
```

*Generated on: 2/11/2026, 5:49:29 pm*