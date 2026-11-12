## 01. Decreasing Increasing Pattern

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/print-pattern3549/1)

### Problem Description

**Task:** Given an integer `n`, generate a sequence following these rules:Start with `n` and repeatedly subtract 5 until the number becomes less than or equal to 0.Then, repeatedly add 5 until the sequence reaches the original number `n`.Solve the problem without using loops.Examples:Input: n = -16

#### Examples

##### Example 1

- **Output:**
```text
[10, 5, 0, 5, 10]
```
- **Explanation:** The value decreases by 5 until it reaches 0:10 - > 5 - > 0. Then, 5 is repeatedly added until it returns to 10: 0 - > 5 - > 10.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-12 21:32:32
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public ArrayList<Integer> pattern(int n) {
        ArrayList<Integer> arr = new ArrayList<>();
        solve(n, arr);
        return arr;
    }

    public void solve(int n, ArrayList<Integer> arr) {
        arr.add(n);

        if (n <= 0) {
            return;
        }

        solve(n - 5, arr);
        arr.add(n);
    }
}
```

*Generated on: 12/11/2026, 9:32:47 pm*