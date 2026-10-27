## 01. All Prime Factors in Sorted Order

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/prime-factorization/1)

### Problem Description

**Task:** Given a number n find the prime factorization of the number.

> **Note:** Print the prime factors in non-decreasing order.

#### Examples

##### Example 1

- **Input:**
```text
n = 100
```
- **Output:**
```text
2 2 5 5
```
- **Explanation:** 100 = 2 * 2 * 5 * 5

##### Example 2

- **Input:**
```text
n = 27
```
- **Output:**
```text
3 3 3
```
- **Explanation:** 27 = 3 * 3 * 3

#### Constraints

- **1.** `2 <= n <= 200`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-27 22:45:07
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public static void printPrimeFactorization(int n) {
        for(int i=2;i<=n;i++)
        {
        while(n%i==0)
        {
            System.out.print(i+" ");
            n=n/i;
        }
        }
        // code here
        
    }
}
```

*Generated on: 27/10/2026, 10:45:46 pm*