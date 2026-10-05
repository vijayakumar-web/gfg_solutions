## 01. Majority Element

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/majority-element-1587115620/1?utm_source=chatgpt.com)

### Problem Description

**Task:** Given an array arr[]. Find the majority element in the array. If no majority element exists, return -1.Note: A majority element in an array is an element that appears strictly more than arr.size()/2 times in the array.Examples:Input: arr[] = [1, 1, 2, 1, 3, 5, 1]

#### Examples

##### Example 1

- **Output:**
```text
-1
```
- **Explanation:** Since, no element is present more than 2/2 times, so there is no majority element.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-05 18:22:00
- **Status:** Correct
- **Marks:** 4

```java
import java.util.HashMap;
class Solution {
    int majorityElement(int arr[]) {
        // import java.util.HashMap
            HashMap<Integer,Integer>map=new HashMap<>();
            for(int i=0;i<arr.length;i++)
            {
                if(map.containsKey(arr[i]))
                {
                    map.put(arr[i],map.get(arr[i])+1);
                }
                else{
                    map.put(arr[i],1);
                }
            }
            int n=arr.length/2;
            for(int i=0;i<arr.length;i++)
            {
                if(map.get(arr[i])>n)
                {
                  return arr[i];
                }
            }
            return-1;
        }
    }
```

*Generated on: 5/10/2026, 6:24:07 pm*