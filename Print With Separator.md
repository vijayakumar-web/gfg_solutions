## 01. Print With Separator

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/print-with-separator/1?page=1&sortBy=submissions)

### Problem Description

**Task:** Given two strings s1 and s2, and a separator symbol separator, print s1 and s2 with separator between them, followed by a new line.Examples :Input: s1 = "Hello", s2 = "World", separator = "@"

#### Examples

##### Example 1

- **Output:**
```text
Geeks-ForExplanation: s1 and s2 are printed with the - symbol in between.
```
- **Explanation:** s1 and s2 are printed with the @ symbol in between.Input: s1 = "Geeks", s2 = "For", separator = "-"

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-31 20:58:32
- **Status:** Correct
- **Marks:** 1

```java
import java.util.Scanner;

class GFG {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String s1 = sc.nextLine();
        String s2 = sc.nextLine();
        String separator = sc.nextLine();
        System.out.println(s1+separator+s2);

        // code here
        
    }
}
```

*Generated on: 31/10/2026, 8:58:56 pm*