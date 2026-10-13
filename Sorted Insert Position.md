## 01. Sorted Insert Position

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/search-insert-position-of-k-in-a-sorted-array/1)

### Problem Description

**Task:** Given a sorted array arr[] (0-index based) of distinct integers and an integer k, find the index of k if it is present in the arr[]. If not, return the index where k should be inserted to maintain the sorted order.Examples :Input: arr[] = [1, 3, 5, 6], k = 5

#### Examples

##### Example 1

- **Output:**
```text
1
```
- **Explanation:** The element 2 is not present in the array, but inserting it at index 1 will maintain the sorted order.Input: arr[] = [2, 6, 7, 10, 14], k = 15Output: 5Explanation: The element 15 is not present in the array, but inserting it after index 4 will maintain the sorted order.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-13 16:46:47
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public int searchInsertK(int arr[], int k) {
        // code here
        int start=0;
        int end=arr.length-1;
        // for(int i=0;i<arr.length;i++)
         while(start<=end)
         {
             int mid=(start+end)/2;
         
         if(k<arr[mid]){
            end=mid-1;
         }
         if(k>arr[mid])
         {
             start=mid+1;
         }
         if(k==arr[mid])
         {
             return mid;
         }
         }
         return start;
    }
}
```

*Generated on: 13/10/2026, 4:47:03 pm*