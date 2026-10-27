## 01. Count Odd and Even

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/count-odd-even/1?utm_source=chatgpt.com)

### Problem Description

**Task:** Given an array arr[] of positive integers. The task is to return the count of the number of odd and even elements in the array.Note: Return two elements where the first one in the count of odd & second one is the count of even.Examples:Input: arr[] = [1, 2, 3, 4, 5]

#### Examples

##### Example 1

- **Output:**
```text
2 0Explanation: There are 2 odd elements (1, 1) and no even elements.Constraints:1 <= arr.size <= 10⁶¹ <= arr[i] <= 10⁶
```
- **Explanation:** There are 3 odd elements (1, 3, 5) and 2 even elements (2 and 4).Input: arr[] = [1, 1]

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (3)

#### Solution 1 (Java)

- **Submitted:** 2026-10-27 08:55:05
- **Status:** Correct
- **Marks:** 0

```java
class Solution {
    public int[] countOddEven(int[] arr) {
        // Code here
        int evecount=0;
        int oddcount=0;
        for(int i=0;i<arr.length;i++)
        {
            if(arr[i]%2==0)
            {
                evecount++;
            }
            else{
            oddcount++;
        }
        }
        return new int[]{oddcount,evecount};
        
    }
}
```

#### Solution 2 (Java)

- **Submitted:** 2026-10-03 08:19:42
- **Status:** Correct
- **Marks:** 0

```java
class Solution {
    public int[] countOddEven(int[] arr) {
        int evencount=0;
        int oddcount=0;
        for(int i=0;i<arr.length;i++)
        {
            if(arr[i]%2==0)
            {
                evencount++;
            }
            else
            {
                oddcount++;
            }
        }
            return new int[]{oddcount,evencount};
    }
}
```

#### Solution 3 (Java)

- **Submitted:** 2026-08-23 15:14:19
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public int[] countOddEven(int[] arr) {
        int evecount=0;
        int oddcount=0;
        for(int i=0;i<arr.length;i++)
        {
        if(arr[i]%2!=0)
        {
            oddcount++;
        }
        else
        {
            evecount++;
        }
        }
        return new int[]{oddcount,evecount};
    }
}
```

*Generated on: 27/10/2026, 8:55:16 am*