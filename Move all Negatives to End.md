## 01. Move all Negatives to End

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/move-all-negative-elements-to-end1813/1?utm_source=chatgpt.com)

### Problem Description

**Task:** Given an unsorted array arr[ ] having both negative and positive integers. Place all negative elements at the end of the array without changing the order of positive elements and negative elements.Note: Don't return any array, just in-place on the array.Examples:Input : arr[] = [1, -1, 3, 2, -7, -5, 11, 6 ]

#### Examples

##### Example 1

- **Output:**
```text
[7, 9, 10, 11, -5, -3, -4, -1]
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-22 09:38:39
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public void segregateElements(int[] arr) {
        int[]temp=new int[arr.length];
        int start=0;
        for(int i=0;i<arr.length;i++)
        {
            if(arr[i]>=0)
            {
                temp[start]=arr[i];
                start++;
            }
            
        }
        for(int i=0;i<arr.length;i++)
        {
            if(arr[i]<0)
            {
                temp[start]=arr[i];
                start++;
            }
        }
        for(int i=0;i<arr.length;i++)
        {
            arr[i]=temp[i];
        }
    }
}
```

*Generated on: 22/10/2026, 9:39:00 am*