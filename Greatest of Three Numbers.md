## 01. Greatest of Three Numbers

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/greatest-of-three-numbers2520/1)

### Problem Description

**Task:** Given three numbers a, b and c. Find the greatest number among them.Examples:Input: a = 10, b = 3, c = 2

#### Examples

##### Example 1

- **Output:**
```text
-2
```
- **Explanation:** -2 is greatest among the three

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-02 17:53:19
- **Status:** Correct
- **Marks:** 1

```java
import java.util.Scanner;

class GFG {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();
        int c = sc.nextInt();
        if(a>b && a>c)
        {
            System.out.print(a);
        }
        if(b>c && b>a)
        {
            System.out.print(b);
        }
        else if(c>b && c>a)
        {
            System.out.print(c);
        }
        // code here
        
    }
}
```

*Generated on: 2/11/2026, 5:53:38 pm*