## 01. At Least Two Greater

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/at-least-two-greater-elements4625/1)

### Problem Description

**Task:** Given an array arr of distinct elements, the task is to return an array of elements that have at least two greater elements.Examples:Input: arr[] = [2, 8, 7, 1, 5]

#### Examples

##### Example 1

- **Output:**
```text
[1, 2, 5]
```
- **Explanation:** Here we return an array contains 1, 2, 5 and we leave two greatest elements 7 & 8. Input: arr[] = [7, -2, 3, 4, 9, -1]Output: [-2, -1, 3, 4]Explanation: Here we return an array contains -2 , -1, 3, 4 and we leave two greatest elements 7 & 9.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n log n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-19 21:03:20
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public ArrayList<Integer> findElements(int[] arr) {
        Arrays.sort(arr);
        ArrayList<Integer>ar=new ArrayList<>();
        for(int i=0;i<arr.length-2;i++)
        {
            ar.add(arr[i]);
        }
        return ar;
        
        // code here
        
    }
}
```

*Generated on: 19/11/2026, 9:03:40 pm*