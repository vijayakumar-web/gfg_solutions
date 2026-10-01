## 01. Missing in Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/missing-number-in-array1416/1?utm_source=chatgpt.com)

### Problem Description

**Task:** You are given an array arr[] of size n - 1 that contains distinct integers in the range from 1 to n (inclusive). This array represents a permutation of the integers from 1 to n with one element missing. Your task is to identify and return the missing element.Examples:Input: arr[] = [1, 2, 3, 5]

#### Examples

##### Example 1

- **Output:**
```text
2
```
- **Explanation:** Only 1 is present so the missing element is 2.Constraints:1 ≤ arr.size() ≤ 10⁶¹ ≤ arr[i] ≤ arr.size() + 1

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (3)

#### Solution 1 (Java)

- **Submitted:** 2026-10-01 19:01:40
- **Status:** Correct
- **Marks:** 0

```java
class Solution {
    int missingNum(int arr[]) {
                int n=arr.length+1;
              long  sum=0;
                long expectedsum=0;
                expectedsum=(long)n*(n+1)/2;
                for(int i=0;i<arr.length;i++)
                {
                    sum+=arr[i];
                }
                return (int)(expectedsum-sum);
            }
        }
```

#### Solution 2 (Java)

- **Submitted:** 2025-07-12 13:23:55
- **Status:** Correct
- **Marks:** 0

```java
import java.util.*;
class Solution {
    int missingNum(int arr[]) {
        Arrays.sort(arr);
            int k=1,i=0;
                for(i=0;i<arr.length;i++)
                {
                 if(arr[i]!=k)
                 {
                     return k;
                 }
                 k++;
                 }
                 return arr[i-1]+1;
            }
        }
```

#### Solution 3 (Java)

- **Submitted:** 2025-07-09 15:25:29
- **Status:** Correct
- **Marks:** 2

```java
class Solution:
    def missingNum(self, arr):
        n=len(arr)+1
        total=n*(n+1)//2
        sum1=sum(arr)
        return total-sum1
       
        # code here
```

*Generated on: 1/10/2026, 7:02:24 pm*