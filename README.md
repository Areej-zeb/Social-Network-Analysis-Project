## Dataset
The dataset consists of three files:
- `social-network-proj-graph.txt` → Defines user connections with weighted edges.
- `social-network-proj-Influences.txt` → Provides influence scores for each user.
- `social-network-proj-LABELS.txt` → Maps user IDs to their names.

---

## Implementation Details

### Part 1: Shortest Path Analysis
- Algorithm: [Dijkstra's Algorithm](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm) (Bonus: [A* Algorithm](https://en.wikipedia.org/wiki/A*_search_algorithm))
- Steps:
  1. Parse the dataset to construct an adjacency list representation.
  2. Apply Dijkstra's (or A* with heuristic).
  3. Output the shortest path & its total weight.

⏳ Time Complexity: O((V + E) log V)

---

### Part 2: Influence Chain Analysis
- Algorithm: Dynamic Programming with DFS
- Steps:
  1. Construct a graph with influence scores from the dataset.
  2. Apply DFS with memoization to compute the longest increasing influence chain
  3. Output the longest chain length & sequence of users

⏳ Time Complexity: O(V + E)

---


Input the start and end users for shortest path computation.
Results & Insights
✅ Find shortest paths to measure connection strength between users.
✅ Identify key influencers in a network based on influence scores.
✅ Visualize influence propagation and user connectivity.

