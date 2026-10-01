## 01. Longest Colored Path

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/longest-colored-path--151454/1)

### Problem Description

**Task:** Given an undirected acyclic graph (tree) with n nodes numbered from 1 to n. Each node is colored either Red (R) or Blue (B).The colors of the nodes are given by a string s of length n, where:s[i] = 'R' means node i + 1 is Red.s[i] = 'B' means node i + 1 is Blue.You are also given a list of n - 1 edges edges[][], where each edges[i] = [u, v] represents an undirected edge between nodes u and v.You can start from any node and traverse along the edges to form a path.A path is called valid if, once you visit a Blue node, you cannot visit any Red node after it on the same path.In other words, a valid path must have the following form:Only Red nodes, orOnly Blue nodes, orSome Red nodes followed by some Blue nodes.A path containing a pattern like Blue - > Red is invalid.Find the maximum number of nodes in a valid path.Examples:Input: s = "RBB", edges = [[1, 2], [1, 3]] Output: 2Explanation: The longest path is either 1 - > 2 or 1 - > 3. In both cases, the length of the path is 2.Input: s = "BB", edges = [[1, 2]]

#### Examples

##### Example 1

- **Output:**
```text
2Explanation: The longest path is 1 - > 2. The length of the path is 2.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (2)

#### Solution 1 (Java)

- **Submitted:** 2026-10-01 11:07:40
- **Status:** Correct
- **Marks:** 0

```java
import java.util.*;

class Solution {

    public int longestPath(String s, int[][] edges) {

        int n = s.length();

        List<Integer>[] graph = new ArrayList[n];

        for (int i = 0; i < n; i++) {
            graph[i] = new ArrayList<>();
        }

        // Build graph
        for (int[] edge : edges) {

            int u = edge[0] - 1;
            int v = edge[1] - 1;

            graph[u].add(v);
            graph[v].add(u);
        }

        int[] dist1 = new int[n];
        int[] dist2 = new int[n];

        Arrays.fill(dist1, -1);
        Arrays.fill(dist2, -1);

        int[] farthest = new int[n];

        boolean[] visited = new boolean[n];

        int answer = 1;

        // Process every same-color component
        for (int start = 0; start < n; start++) {

            if (visited[start])
                continue;

            char color = s.charAt(start);

            List<Integer> component = new ArrayList<>();

            // Find one endpoint of this component
            int end1 = bfs(
                    start,
                    color,
                    s,
                    graph,
                    dist1,
                    component
            );

            // Mark component as visited
            for (int node : component) {
                visited[node] = true;
                dist1[node] = -1;
            }

            // Find other endpoint
            int end2 = bfs(
                    end1,
                    color,
                    s,
                    graph,
                    dist1,
                    new ArrayList<>()
            );

            // BFS from other endpoint
            bfs(
                    end2,
                    color,
                    s,
                    graph,
                    dist2,
                    new ArrayList<>()
            );

            // Longest same-color path
            answer = Math.max(
                    answer,
                    dist1[end2] + 1
            );

            // Maximum same-color distance from every node
            for (int node : component) {

                farthest[node] =
                        Math.max(dist1[node], dist2[node]);

                dist1[node] = -1;
                dist2[node] = -1;
            }
        }

        // Try every edge connecting different colors
        for (int[] edge : edges) {

            int u = edge[0] - 1;
            int v = edge[1] - 1;

            if (s.charAt(u) != s.charAt(v)) {

                int path =
                        farthest[u]
                        + farthest[v]
                        + 2;

                answer = Math.max(answer, path);
            }
        }

        return answer;
    }


    private int bfs(
            int start,
            char color,
            String s,
            List<Integer>[] graph,
            int[] dist,
            List<Integer> nodes
    ) {

        Queue<Integer> queue = new LinkedList<>();

        dist[start] = 0;
        queue.add(start);
        nodes.add(start);

        int farthestNode = start;

        while (!queue.isEmpty()) {

            int u = queue.poll();

            for (int v : graph[u]) {

                // Different color -> don't enter
                if (s.charAt(v) != color)
                    continue;

                // Already visited
                if (dist[v] != -1)
                    continue;

                dist[v] = dist[u] + 1;

                queue.add(v);
                nodes.add(v);

                if (dist[v] > dist[farthestNode]) {
                    farthestNode = v;
                }
            }
        }

        return farthestNode;
    }
}
```

#### Solution 2 (Java)

- **Submitted:** 2026-10-01 11:00:22
- **Status:** Correct
- **Marks:** 8

```java
import java.util.*;

class Solution {

    public int longestPath(String s, int[][] edges) {

        int n = s.length();

        List<Integer>[] graph = new ArrayList[n];

        for (int i = 0; i < n; i++) {
            graph[i] = new ArrayList<>();
        }

        // Build graph
        for (int[] edge : edges) {

            int u = edge[0] - 1;
            int v = edge[1] - 1;

            graph[u].add(v);
            graph[v].add(u);
        }

        int[] dist1 = new int[n];
        int[] dist2 = new int[n];

        Arrays.fill(dist1, -1);
        Arrays.fill(dist2, -1);

        int[] farthest = new int[n];

        boolean[] visited = new boolean[n];

        int answer = 1;

        // Process every same-color component
        for (int start = 0; start < n; start++) {

            if (visited[start])
                continue;

            char color = s.charAt(start);

            List<Integer> component = new ArrayList<>();

            // Find one endpoint of this component
            int end1 = bfs(
                    start,
                    color,
                    s,
                    graph,
                    dist1,
                    component
            );

            // Mark component as visited
            for (int node : component) {
                visited[node] = true;
                dist1[node] = -1;
            }

            // Find other endpoint
            int end2 = bfs(
                    end1,
                    color,
                    s,
                    graph,
                    dist1,
                    new ArrayList<>()
            );

            // BFS from other endpoint
            bfs(
                    end2,
                    color,
                    s,
                    graph,
                    dist2,
                    new ArrayList<>()
            );

            // Longest same-color path
            answer = Math.max(
                    answer,
                    dist1[end2] + 1
            );

            // Maximum same-color distance from every node
            for (int node : component) {

                farthest[node] =
                        Math.max(dist1[node], dist2[node]);

                dist1[node] = -1;
                dist2[node] = -1;
            }
        }

        // Try every edge connecting different colors
        for (int[] edge : edges) {

            int u = edge[0] - 1;
            int v = edge[1] - 1;

            if (s.charAt(u) != s.charAt(v)) {

                int path =
                        farthest[u]
                        + farthest[v]
                        + 2;

                answer = Math.max(answer, path);
            }
        }

        return answer;
    }


    private int bfs(
            int start,
            char color,
            String s,
            List<Integer>[] graph,
            int[] dist,
            List<Integer> nodes
    ) {

        Queue<Integer> queue = new LinkedList<>();

        dist[start] = 0;
        queue.add(start);
        nodes.add(start);

        int farthestNode = start;

        while (!queue.isEmpty()) {

            int u = queue.poll();

            for (int v : graph[u]) {

                // Different color -> don't enter
                if (s.charAt(v) != color)
                    continue;

                // Already visited
                if (dist[v] != -1)
                    continue;

                dist[v] = dist[u] + 1;

                queue.add(v);
                nodes.add(v);

                if (dist[v] > dist[farthestNode]) {
                    farthestNode = v;
                }
            }
        }

        return farthestNode;
    }
}
```

*Generated on: 1/10/2026, 11:07:59 am*