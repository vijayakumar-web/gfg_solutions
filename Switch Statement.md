## 01. Switch Statement

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/switch-statement/1)

### Problem Description

**Task:** Given a number n, use a switch statement to return "One" if the given number is equal to 1, "Two" if the number is 2 and so on till 9 ("Nine") else return "Unknown"(without quotes). Examples:Input: n = 10

#### Examples

##### Example 1

- **Output:**
```text
One
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-12 22:21:53
- **Status:** Correct
- **Marks:** 1

```java
import java.util.Scanner;
    
    class GFG {
        public static void main(String[] args) {
            Scanner sc = new Scanner(System.in);
            int n = sc.nextInt();
            switch(n)
            {
            case 1:
                System.out.println("One");
                break;
            case 2:
                System.out.println("Two");
                break;
            case 3:
                System.out.println("Three");
                break;
            case 4:
                System.out.println("Four");
                break;
            case 5:
                System.out.println("Five");
                break;
            case 6:
                System.out.println("Six");
                break;
            case 7:
                System.out.println("Seven");
                break;
            case 8:
                System.out.println("Eight");
                break;
            case 9:
                System.out.println("Nine");
                break;
            default:
                System.out.println("Unknown");
            }
        }
    }
```

*Generated on: 12/10/2026, 10:22:08 pm*