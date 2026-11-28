## 01. Compare Two Numbers

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/compare-two-numbers/1?selectedLang=java)

### Problem Description

**Task:** Given two integers a and b, print 1 if a is greater than b; otherwise, print 0.Example :Input: a = 4, b = 6

#### Examples

##### Example 1

- **Output:**
```text
0Explanation: Since both numbers are equal, a is not greater than b.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-28 08:36:14
- **Status:** Correct
- **Marks:** 1

```java
import java.util.Scanner;

class GFG {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        // code here
        if(a>b)
        {
            System.out.println(1);
        }
        else
        {
        System.out.println(0);
        }
    }
}
```

*Generated on: 28/11/2026, 8:36:28 am*