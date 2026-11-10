## 01. Reverse Array in Groups

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/reverse-array-in-groups0255/1)

### Problem Description

**Task:** Given an integer array arr[] and an integer k, reverse every consecutive group of k elements. If fewer than k elements remain at the end, reverse all of them.Examples:Input: arr[] = [1, 2, 3, 4, 5], k = 3Output: [3, 2, 1, 5, 4]

#### Examples

##### Example 1

- **Explanation:** First group consists of elements 1, 2, 3. Second group consists of 4, 5.Input: arr[] = [5, 6, 8, 9], k = 5Output: [9, 8, 6, 5]Explnation: Since k is greater than the number of remaining elements, the entire array is reversed.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-10 10:44:12
- **Status:** Correct
- **Marks:** 4

```java
class Solution {
    public void reverseInGroups(int[] arr, int k) {
        for(int i=0;i<arr.length;i+=k)
        {
            int start=i;
            int end=Math.min(i+k-1,arr.length-1);
            while(start<end)
            {
                int temp=arr[start];
                arr[start]=arr[end];
                arr[end]=temp;
                start++;
                end--;
            }
            
            
        }
  
        
    }
}
```

*Generated on: 10/11/2026, 10:44:30 am*