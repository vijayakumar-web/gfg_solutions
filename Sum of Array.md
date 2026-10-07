## 01. Sum of Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/sum-all-array-elements/1)

### Problem Description

**Task:** Given an integer array arr[], return the sum of all elements of arr.Examples:Input: arr[] = [1, 2, 3, 4]

#### Examples

##### Example 1

- **Output:**
```text
10
```
- **Explanation:** 1 + 2 + 3 + 4 = 10.

##### Example 2

- **Input:**
```text
arr[] = [1, 3, 3]
```
- **Output:**
```text
7
```
- **Explanation:** 1 + 3 + 3 = 7.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-07 13:03:36
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public int arraySum(int arr[]) {
        int sum=0;
        for(int i=0;i<arr.length;i++)
        {
            sum+=arr[i];
        }
        return sum;
        
    }
}
```

*Generated on: 7/10/2026, 1:04:07 pm*