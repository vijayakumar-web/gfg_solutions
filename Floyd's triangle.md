## 01. Floyd's triangle

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/floyds-triangle1222/1)

### Problem Description

**Task:** Given a number n, print Floyd's triangle with n lines.
Floyd’s Triangle is a pattern of consecutive natural numbers arranged in rows, where the i-th row contains i numbers.

#### Examples

##### Example 1

- **Input:**
```text
n = 4 1 2 3 4 5 6 7 8 9 10
```
- **Explanation:** The triangle has 4 rows. Numbers start from 1 and increase sequentially across rows, and each row i contains i elements.

##### Example 2

- **Input:**
```text
n = 5 Output: 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15
```
- **Explanation:** The triangle has 4 rows, and each row i contains i numbers.

#### Constraints

- **1.** `1 <= n <= 100`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-07 19:30:11
- **Status:** Correct
- **Marks:** 1

```java
import java.util.Scanner;

class GFG {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int num=1;
        for(int i=1;i<=n;i++)
        {
        for(int j=1;j<=i;j++)
        {
            System.out.print(num+" ");
            num++;
        }
        System.out.println();
        }
    }
}
```

*Generated on: 7/10/2026, 7:30:29 pm*