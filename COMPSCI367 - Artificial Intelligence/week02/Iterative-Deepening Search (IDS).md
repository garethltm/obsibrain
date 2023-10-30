### Summary
- try all possible depth limits in turn
- Combines benefits of [[Depth-First Search (DFS)]] and [[Breadth-First Search (BFS)]]
	- **[[Depth-First Search (DFS)]] (low memory - [[Space Complexity]])** 
	- **[[Breadth-First Search (BFS)]] ([[optimal]] and [[complete]])** 
	==by doing a series of **[[Depth-Limited Search (DLS)]]** to depth 1,2,3, etc.==
- early [[state(s)]] will be expanded multiple times, but that might not matter too much because most of the nodes are near the leaves
- similar to [[Depth-Limited Search (DLS)]] in terms of [[Space Complexity]] & [[Time Complexity]]
## Finding max path cost
- Diameter of the [[state space]] - the maximum [[path cost]] between any 2 nodes
	- this would be a good candidate for a depth limit but it may be difficult to determine in advance
- Therefore, it can be very difficult to decide upon a [[Depth-Limited Search (DLS)]] for search
## Properties
- [[Complete]]
    - Yes
- [[Time Complexity]]
    - $O(b^d)$ nodes at the top level are expanded once, nodes at the next level twice,...
- [[Space Complexity]]
    - $O(bd)$
- [[Optimal]]
    - Yes, if step costs are identical