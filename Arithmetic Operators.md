## 01. Arithmetic Operators

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/arithmetic-operators/1)

### Problem Description

**Task:** Given two integer variables x and y, perform the following operations:p: Addition of x and yq: Subtraction of y from xr: Multiplication of x and ys: Floating-point division of x by yt: Integer division of x by yu: Modulo (remainder when x is divided by y)Examples:Input: x = 1, y = 2

#### Examples

##### Example 1

- **Output:**
```text
3 -1 2 0.500 0 1
```
- **Explanation:** The given operations are performed:Addition of x and y = 3Subtraction of y from x = -1Multiplication of x and y = 2Floating-point division of x by y = 0.500Integer division of x by y = 0Modulo of x and y = 1Hence, the output is 3 -1 2 0.500 0 1.

##### Example 2

- **Input:**
```text
x = 3, y = 4
```
- **Output:**
```text
7 -1 12 0.750 0 3
```
- **Explanation:** The given operations are performed.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-15 19:28:35
- **Status:** Correct
- **Marks:** 1

```java
import java.util.*;

class GFG {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int x = sc.nextInt();
        int y = sc.nextInt();

        int p = x + y;
        int q = x - y;
        int r = x * y;
        double s = (double) x / y;
        int t = x / y;
        int u = x % y;

        System.out.printf("%d %d %d %.3f %d %d", p, q, r, s, t, u);

        sc.close();
    }
}
```

*Generated on: 15/10/2026, 7:28:54 pm*