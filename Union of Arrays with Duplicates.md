## 01. Union of Arrays with Duplicates

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/union-of-two-arrays3538/1?utm_source=chatgpt.com)

### Problem Description

**Task:** You are given two arrays a[] and b[], return the Union of both the arrays in any order.The Union of two arrays is a collection of all distinct elements present in either of the arrays. If an element appears more than once in one or both arrays, it should be included only once in the result.Note: Elements of a[] and b[] are not necessarily distinct.Note that, You can return the Union in any order but the driver code will print the result in sorted order only.Examples:Input: a[] = [1, 2, 3, 2, 1], b[] = [3, 2, 2, 3, 3, 2]

#### Examples

##### Example 1

- **Output:**
```text
[1, 2, 3]
```
- **Explanation:** Union set of both the arrays will be 1, 2 and 3.

##### Example 2

- **Input:**
```text
a[] = [1, 2, 3], b[] = [4, 5, 6] Output: [1, 2, 3, 4, 5, 6]
```
- **Explanation:** Union set of both the arrays will be 1 and 2.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n + m)
- **Expected Auxiliary Space Complexity:** O(n + m)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-10-05 19:20:25
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public static ArrayList<Integer> findUnion(int[] a, int[] b) {
        HashSet<Integer>set=new HashSet<>();
        for(int i=0;i<a.length;i++)
        {
            set.add(a[i]);
        }
        for(int j=0;j<b.length;j++)
        {
            set.add(b[j]);
        }
        ArrayList<Integer>result=new ArrayList<>();
        for(Integer x:set)
        {
            result.add(x);
            
        }
        return result;
    }
}
```

*Generated on: 5/10/2026, 7:20:44 pm*