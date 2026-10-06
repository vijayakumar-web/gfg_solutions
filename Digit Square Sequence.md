## 01. Digit Square Sequence

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/happy-number1408/1)

### Problem Description

**Task:** Given a positive integer n, generate a sequence by repeatedly replacing the current number with the sum of the squares of its digits.
Find whether this sequence eventually reaches 1. Return true if it does, otherwise return false.

#### Examples

##### Example 1

- **Input:**
```text
n = 19
```
- **Output:**
```text
true 19 = 1² + 9² = 82 82 = 8² + 2² = 68 68 = 6² + 8² = 100 100 = 1² + 0² + 0² = 1 Since the sequence reaches 1, return true.
```

##### Example 2

- **Input:**
```text
n = 20
```
- **Output:**
```text
false
```
- **Explanation:** 20 = 2² + 0² = 4 4 = 4² = 16 16 = 1² + 6² = 37 37 = 3² + 7² = 58 58 = 5² + 8² = 89 89 = 8² + 9² = 145 145 = 1² + 4² + 5² = 42 42 = 4² + 2² = 20 The sequence enters a cycle without reaching 1, so return false.

#### Constraints

- **1.** `1 ≤ n ≤ 10⁹`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-06 12:23:45
- **Status:** Correct
- **Marks:** 2

```java
import java.util.HashSet;
class Solution {
    public boolean reachesOne(int n) {
                HashSet<Integer> set = new HashSet<>();

                while (n != 1) {

                    // Check if the number is already seen
                    if (set.contains(n)) {
                        return false;
                    }

                    // Store the number
                    set.add(n);

                    // Calculate sum of squares of digits
                    int sum = 0;

                    while (n > 0) {
                        int digit = n % 10;
                        n = n / 10;

                        sum = sum + digit * digit;
                    }

                    // Use the calculated sum as the new number
                    n = sum;
                }

                return true;
    }
}
```

*Generated on: 6/10/2026, 12:24:24 pm*