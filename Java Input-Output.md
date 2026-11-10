## 01. Java Input/Output

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/java-inputoutput0118/1)

### Problem Description

**Task:** Given a string S and an integer number N, print the output in the form: "The input string :S" and "The input integer :N" in the two separate lines.
Example 1:

#### Examples

##### Example 1

- **Explanation:** On the first line we have to print "The input string :S" where S = 'GeeksforGeeks'. On the second line, we have to print "The input integer :N" Where N is 20. Example 2:

##### Example 2

- **Explanation:** On the first line, we have to print "The input string :S" where S = 'Power'. On the second line, we have to print "The input integer :N" Where N is 50. Your Task: You don't need to read input. Your task is to complete the function printIntString() which takes the String S and an Integer N as input parameters and print two Strings on separate lines as mentioned above. Expected Time Complexity: O(1)Expected Auxiliary Space: O(1)

#### Constraints

- **1.** `1 <= |string length| <= 10³`
- **2.** `1 <= N <= 10⁴`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** Not found
- **Expected Auxiliary Space Complexity:** Not found

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-10 10:54:04
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    static void printIntString(String S, int N) {
        System.out.println("The input string :"+S);
        System.out.println("The input integer :"+N);
        // code here
        
    }
}
```

*Generated on: 10/11/2026, 11:00:10 am*