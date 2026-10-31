## 01. Calculator

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/calculator--172632/1)

### Problem Description

**Task:** Given two numbers a and b. You need to perform basic mathematical operations on them. You will be provided an integer named as optr.
If the operator equals to 1 add a and b, then print the result.
If the operator equals to 2 subtract b from a, then print the result.
If the operator equals to 3 multiply a and b, then print the result.
If the operator equals to any other number, print "Invalid Input"(without quotes).

> **Note:** Do not add a new line at the end.

#### Examples

##### Example 1

- **Input:**
```text
a = 1, b = 2, optr = 3
```
- **Output:**
```text
2
```
- **Explanation:** 1 * 2 = 2

##### Example 2

- **Input:**
```text
a = 2, b = 2, optr = 2
```
- **Output:**
```text
0
```
- **Explanation:** 2 - 2 = 0

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-31 21:49:37
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public void calculate(int a, int b, int optr) {
        if(optr==1)
        {
            System.out.print(a+b);
        }
        else if(optr==2)
        {
            System.out.print(a-b);
        }
        else if(optr==3)
        {
            System.out.print(a*b);
        }
        else 
        {
            System.out.print("Invalid Input");
        }
        // code here
    }
}
```

*Generated on: 31/10/2026, 10:04:22 pm*