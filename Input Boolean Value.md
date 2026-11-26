## 01. Input Boolean Value

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/input-boolean-value/1?selectedLang=java)

### Problem Description

**Task:** Take a boolean value a as an input. The program should display its numeric representation:
1 for "true"
0 for "false"

#### Examples

##### Example 1

- **Input:**
```text
a = true
```
- **Output:**
```text
1
```

##### Example 2

- **Input:**
```text
a = false
```
- **Output:**
```text
0
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-26 09:55:45
- **Status:** Correct
- **Marks:** 1

```java
import java.util.Scanner;

class GFG {
    public static void main(String[] args) {
        // Scanner sc = new Scanner(System.in);
        Scanner sc=new Scanner(System.in);
        boolean a=sc.nextBoolean();
        // boolean a;
        if(a==true)
        {
            System.out.print(1);
        }
        else
        {
            System.out.print(0);
        }
        // code here


        // Printing numeric representation
        // System.out.print(a ? 1 : 0);
    }
}
```

*Generated on: 26/11/2026, 9:55:54 am*