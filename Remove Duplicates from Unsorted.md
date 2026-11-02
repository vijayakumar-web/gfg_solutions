## 01. Remove Duplicates from Unsorted

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/remove-duplicates-from-unsorted-array4141/1)

### Problem Description

**Task:** Given an array arr[] of integers which may or may not contain duplicate elements. Your task is to remove duplicate elements. Your result should have elements according their first appearance in the input array.Examples:Input: arr[] = [1, 2, 3, 1, 4, 2]

#### Examples

##### Example 1

- **Output:**
```text
[1, 2, 3, 4]Explanation: There is no duplicate element.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-02 18:07:14
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    static ArrayList<Integer> removeDuplicate(int arr[]) {
        LinkedHashSet<Integer>set=new LinkedHashSet<>();
        for(int i=0;i<arr.length;i++)
        {
            set.add(arr[i]);
        }
        // Arrays.sort(set);
        return new ArrayList<>(set);
     
        
    }
}
```

*Generated on: 2/11/2026, 6:07:35 pm*