## 01. Count Distinct in Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/find-distinct-elements--130928/1)

### Problem Description

**Task:** Given an integer array arr[], return the count of all the distinct elements in an arrayExamples:Input: arr[] = [2, 2, 3, 2]

#### Examples

##### Example 1

- **Output:**
```text
5Explanation: Distinct elements are {12, 1, 14, 3, 16}Input: arr[] = [1, 1, 1, 1]Output: 1Explanation: Only one distinct element {1}
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-19 20:37:39
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public int countDistinct(int arr[]) {
        HashMap<Integer,Integer>map=new HashMap<>();
        for(int i=0;i<arr.length;i++)
        {
            if(map.containsKey(arr[i]))
            {
                map.put(arr[i], map.get(arr[i]) + 1);
            }
            else
            {
                map.put(arr[i],1);
            }
        }
        return map.size();
        // code here
        
    }
}
```

*Generated on: 19/11/2026, 8:38:00 pm*