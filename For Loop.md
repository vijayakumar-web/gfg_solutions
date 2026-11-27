## 01. For Loop

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/java-loops-set-11726/1?selectedLang=java)

### Problem Description

**Task:** Given a number n, print the first n positive even numbers in increasing order in a single line using a for loop.Examples:Input: n = 2

#### Examples

##### Example 1

- **Output:**
```text
2 4 6 8 10 12
```
- **Explanation:** The first 6 positive even numbers are 2, 4, 6, 8, 10 and 12.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-27 06:53:26
- **Status:** Correct
- **Marks:** 1

```java
import java.util.Scanner;

class GFG {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        for(int i=1;i<=n;i++)
        {
         
                System.out.print(i*2+" ");
            }
        
    }
}
```

*Generated on: 27/11/2026, 6:53:44 am*