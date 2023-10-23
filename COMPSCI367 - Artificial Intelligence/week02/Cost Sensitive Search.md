- [[Depth-First Search (DFS)]] is not [[optimal]]
- [[Breadth-First Search (BFS)]] finds the shortest [[path(s)]] in terms of number of [[action(s)]]. It does not find the least-cost [[path(s)]]

- [[Uniform-Cost Search (UCS) (Lowest-Cost-First Search)]] is similar to [[Breadth-First Search (BFS)]], but sorts the [[queue]] using the [[path(s)]] cost
    - Expands the lowest [[path(s)]] cost
    - The good: [[Uniform-Cost Search (UCS) (Lowest-Cost-First Search)]] is [[Complete]] and [[Optimal]]
    - The bad: explores options in every “direction”
    - No information about the goal location