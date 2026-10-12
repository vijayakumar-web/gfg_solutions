## 01. While Loop

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/while-loop/1)

### Problem Description

**Task:** Given a number x, print the numbers from x to 0 in decreasing order in a single line.

#### Examples

##### Example 1

- **Input:**
```text
x = 3
```
- **Output:**
```text
3 2 1 0
```
- **Explanation:** Numbers in decreasing order from 3 are 3 2 1 0.

##### Example 2

- **Input:**
```text
x = 5Output: 5 4 3 2 1 0Explanation: Numbers in decreasing order from 5 are 5 4 3 2 1 0.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-12 13:54:39
- **Status:** Correct
- **Marks:** 1

```java
import java.util.Scanner;

class GFG {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int x = sc.nextInt();
        while(x>=0)
        {
            System.out.print(x+" ");
            x--;
        }
        // code here
        
    }
}
```

*Generated on: 12/10/2026, 1:54:56 pm*