## 01. Smallest Positive Missing

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/smallest-positive-missing-number-1587115621/1)

### Problem Description

**Task:** You are given an integer array arr[]. Your task is to find the smallest positive number missing from the array.Note: Positive number starts from 1. The array can have negative integers too.Examples:Input: arr[] = [2, -3, 4, 1, 1, 7]

#### Examples

##### Example 1

- **Output:**
```text
3
```
- **Explanation:** Smallest positive missing number is 3.

##### Example 2

- **Input:**
```text
arr[] = [5, 3, 2, 5, 1]
```
- **Output:**
```text
1
```
- **Explanation:** Smallest positive missing number is 1.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-02 18:25:59
- **Status:** Correct
- **Marks:** 4

```java
class Solution {
    public int missingNumber(int[] arr) {
        HashSet<Integer>set=new HashSet<>();
        for(int i=0;i<arr.length;i++)
        {
            if(arr[i]>0)
            {
            set.add(arr[i]);
            }
        }
        int positive=1;
        while(set.contains(positive))
        {
            positive++;
            
        }
        return positive;
            
       
        
    }
}
```

*Generated on: 2/11/2026, 6:26:16 pm*