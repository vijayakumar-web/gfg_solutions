## 01. Nth Fibonacci Using Recursion

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/fibonacci-using-recursion/1)

### Problem Description

**Task:** Given a number n, return the n^th Fibonacci number.

> **Note:** If F(n) is n^th fibonacci number then , F(n) = F(n-1) + F(n-2) ; where F(0) = 0 and F(1) = 1Example:

#### Examples

##### Example 1

- **Input:**
```text
n = 3
```
- **Output:**
```text
2
```
- **Explanation:** The Fibonacci sequence starts as 0, 1, 1, 2, 3, 5... The 3rd Fibonacci number is 2.

##### Example 2

- **Input:**
```text
n = 5
```
- **Output:**
```text
5
```
- **Explanation:** The sequence is 0, 1, 1, 2, 3, 5... The 5th Fibonacci number is 5.

#### Constraints

- **1.** `1 ≤ n ≤ 20`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(2^n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-06 11:49:45
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    static int nthFibonacci(int n) {
        // code here
        int first=0;
        int second=1;
        for(int i=0;i<n;i++)
        {
        int third=first+second;
        first=second;
        second=third;
        // return third;
}
return first;
}
}
```

*Generated on: 6/11/2026, 11:49:59 am*