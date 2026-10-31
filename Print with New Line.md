## 01. Print with New Line

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/the-new-line/1)

### Problem Description

**Task:** There is a string "Geeks for Geeks", print each word on a separate line.

> **Note:** No input required for this problem.

#### Examples

##### Example 1

- **Input:**
```text
Not Required
```
- **Output:**
```text
Geeks for Geeks
```
- **Explanation:** Each word is printed on a separate line.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-31 20:20:44
- **Status:** Correct
- **Marks:** 1

```java
class GFG {
    public static void main(String[] args) {
        String s="Geeks for Geeks";
        String[]words=s.split(" ");
        for(int i=0;i<words.length;i++){
        System.out.print(words[i]);
        if(i<words.length-1)
        {
            System.out.print("\n");
        }
        
     
        
    }
}
}
```

*Generated on: 31/10/2026, 8:21:03 pm*