## 01. Magic number (programming)

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/sort-an-array-of-0s-1s-and-2s4231/1?utm_source=chatgpt.com)

### Problem Description

**Task:** Given an array arr[] containing only 0s, 1s, and 2s. Sort the array in ascending order. Examples:Input: arr[] = [0, 1, 2, 0, 1, 2]

#### Examples

##### Example 1

- **Output:**
```text
[0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 2, 2]
```
- **Explanation:** 0s, 1s and 2s are segregated into ascending order.Follow up: Could you come up with a one-pass algorithm using only constant extra space?

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (Java)

- **Submitted:** 2026-11-02 15:11:46
- **Status:** Correct
- **Marks:** 0

```java
class Solution {
    public void sort012(int[] arr) {
        Arrays.sort(arr);
        // code here
        
    }
}
```

#### Solution 2 (Java)

- **Submitted:** 2025-08-05 15:11:55
- **Status:** Correct
- **Marks:** 4

```java
class Solution {
    public void sort012(int[] arr) {
    Arrays.sort(arr);
        
    }
}
```

*Generated on: 2/11/2026, 3:12:25 pm*