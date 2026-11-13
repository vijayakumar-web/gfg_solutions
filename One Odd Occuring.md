## 01. One Odd Occuring

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/find-the-odd-occurence4820/1)

### Problem Description

**Task:** Given an array of arr[] positive integers where all numbers occur even number of times except one number which occurs odd number of times. Return that number.Examples:Input:arr[] = [1, 2, 3, 2, 3, 1, 3]

#### Examples

##### Example 1

- **Output:**
```text
3
```
- **Explanation:** 3 occurs three times.

##### Example 2

- **Input:**
```text
arr[] = [5, 7, 2, 7, 5, 2, 5]
```
- **Output:**
```text
5
```
- **Explanation:** 5 occurs three times.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-13 10:24:17
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    // Method to find the element with odd occurrence in given array
    int getOddOccurrence(int[] arr) {
        HashMap<Integer,Integer>map=new HashMap<>();
        for(int i=0;i<arr.length;i++)
        {
            if(map.containsKey(arr[i]))
            {
                map.put(arr[i],map.get(arr[i])+1);
            }
            else
            {
                map.put(arr[i],1);
            }
        }
        for(int key:map.keySet())
        {
            if(map.get(key)%2!=0)
            {
                return key;
                
            }
        }
        return-1;
        
        // code here
        
    }
}
```

*Generated on: 13/11/2026, 10:24:29 am*