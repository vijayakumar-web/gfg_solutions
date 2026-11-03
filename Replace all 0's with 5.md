## 01. Replace all 0's with 5

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/replace-all-0s-with-5/1)

### Problem Description

**Task:** You are given an integer n. You need to convert all zeroes of n to 5. Examples:Input: n = 1004

#### Examples

##### Example 1

- **Output:**
```text
1554
```
- **Explanation:** There are two zeroes in 1004 on replacing all zeroes with 5, the new number will be 1554.

##### Example 2

- **Input:**
```text
n = 121
```
- **Output:**
```text
121
```
- **Explanation:** Since there are no zeroes in 121, the number remains as 121.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(k)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-03 09:49:24
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
        public int convertFive(int n) {
            if(n==0)
            {
                return 5;
            }
            int digit=0;
            int res=0;
            while(n!=0)
            {
                digit=n%10;
                n=n/10;
                if(digit==0)
                {
                    digit=5;
                }
                res=res*10+digit;
            }
        int rev=0;
        int dig=0;
        while(res!=0)
        {
            dig=res%10;
            rev=rev*10+dig;
            res=res/10;
        
        }
        return rev;
        }
    }
```

*Generated on: 3/11/2026, 9:49:42 am*