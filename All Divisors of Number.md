## 01. All Divisors of Number

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/all-divisors-of-a-number/1)

### Problem Description

**Task:** Given an integer n, return all the divisors of n in the ascending order. Examples:Input : n = 20

#### Examples

##### Example 1

- **Output:**
```text
1 2 4 5 10 20
```
- **Explanation:** 20 is completely divisible by 1, 2, 4, 5, 10 and 20.

##### Example 2

- **Input:**
```text
n = 21191
```
- **Output:**
```text
1 21191
```
- **Explanation:** As 21191 is a prime number, it has only 2 factors(1 and the number itself).

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(sqrt(n))
- **Expected Auxiliary Space Complexity:** O(sqrt(n))

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-28 08:32:35
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
     public ArrayList<Integer> getDivisors(int n) {

         ArrayList<Integer> a = new ArrayList<>();

         for(int i = 1; i * i <= n; i++)
         {
             if(n % i == 0)
             {
                 a.add(i);

                 if(i != n / i)
                 {
                     a.add(n / i);
                 }
             }
         }

         Collections.sort(a);

         return a;
     }
 }
```

*Generated on: 28/11/2026, 8:33:01 am*