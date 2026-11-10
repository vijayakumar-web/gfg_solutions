## 01. Common Elements

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/common-elements5420/1)

### Problem Description

**Task:** Given two integer arrays a[] and b[], return an array containing all elements common to both arrays in sorted order.
If an element appears multiple times in both arrays, it should appear in the output as many times as it is common to both arrays.

#### Examples

##### Example 1

- **Input:**
```text
a[] = [3, 4, 2, 2, 4] , b[] = [3, 2, 2, 7]
```
- **Output:**
```text
[2, 2, 3]
```
- **Explanation:** The common elements in sorted order are 2, 2, 3.

##### Example 2

- **Input:**
```text
a[] = [3, 6, 1, 7, 9, 8, 2, 2] , b[] = [9, 7, 3, 4, 9]Output: [3, 7, 9]Explanation: The common elements in sorted order are 3, 7, 9.
```

#### Constraints

- **1.** `1 ≤ a.size(), b.size() ≤ 10⁵¹ ≤ a[i], b[i] ≤ 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O((n+m)*log(n+m))
- **Expected Auxiliary Space Complexity:** O(n + m)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-10 11:28:46
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
     public static ArrayList<Integer> commonElements(int a[], int b[]) {

         ArrayList<Integer> arr = new ArrayList<>();

         Arrays.sort(a);
         Arrays.sort(b);

         int i = 0;
         int j = 0;

         while(i < a.length && j < b.length)
         {
             if(a[i] == b[j])
             {
                 arr.add(a[i]);
                 i++;
                 j++;
             }
             else if(a[i] < b[j])
             {
                 i++;
             }
             else
             {
                 j++;
             }
         }

         return arr;
     }
 }
```

*Generated on: 10/11/2026, 11:28:57 am*