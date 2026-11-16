## 01. Repeated Integer Division by 2

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/geek-and-coffee-shop5721/1)

### Problem Description

**Task:** Given two integers n and m, halve n exactly m - 1 times using integer division. Return the resulting value.

#### Examples

##### Example 1

- **Input:**
```text
n = 100, m = 4
```
- **Output:**
```text
12
```
- **Explanation:** The sequence of numbers is 100, 50, 25, 12.

##### Example 2

- **Input:**
```text
n = 10, m = 5
```
- **Output:**
```text
0
```
- **Explanation:** The sequence is 10, 5, 2, 1 and 0.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-16 22:36:28
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public int mthHalf(int n, int m) {
        for(int i=0;i<m-1;i++)
        {
            n=n/2;
        }
        return n;
        // code here
        
    }
}
```

*Generated on: 16/11/2026, 10:36:46 pm*