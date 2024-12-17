### Summary
- always expand node at deepest level of tree and when search hits a dead-end return back to expand nodes at a shallower level
- can be implemented using a [[Stack]] of explored + [[frontier (open list, fringe)]] nodes
- at any point [[Depth-First Search (DFS)]] stores single [[path(s)]] from root to leaf
    - together with any remaining unexpanded siblings of nodes along [[path(s)]]
- stop when node with [[Goal(s) - Goal State(s)]] is expanded
![[Pasted image 20231022032622.png]]
- Last In First Out
- expands one of the nodes at the deepest level of the tree
## Implementation
- implementing the [[frontier (open list, fringe)]] as a [[Stack]]
    - can alternatively be implemented by recursive function calls
- in [[Depth-First Search (DFS)]], like [[Breadth-First Search (BFS)]], the order in which the [[path(s)]] are expanded does not depend on the [[Goal(s) - Goal State(s)]]
## Properties
1. [[Complete]]
    - No - fails in infinite-depth spaces, spaces with loops
        - we need to modify to avoid repeated [[State(s)]] along [[path(s)]] in finite spaces
2. [[Time Complexity]]
    - $O(b^m)$
	    - m = maximum depth of [[Search Tree]]
	    - b = [[branching factor(s)]]
        - terrible if m is much larger than b
        - but if [[solution(s)]] are dense, can be much faster than [[Breadth-First Search (BFS)]]
3. [[Space Complexity]]
    - $O(bm)$
	    - linear space
4. [[Optimal]]
    - No, can be [[suboptimal]] [[solution(s)]] first
	    - there is a chance that [[Depth-First Search (DFS)]] can hit a [[Goal(s) - Goal State(s)]] due to random chance as [[Breadth-First Search (BFS)]] would systematically go through the search by levels

>[[Depth-First Search (DFS)]] is considered a memory efficient algorithm as it only stores the nodes that is currently being generated

## Analysis
- In cases where problem has many [[solution(s)]], [[Depth-First Search (DFS)]] may outperform [[Breadth-First Search (BFS)]] because there is a good chance it will find a [[solution(s)]] after exploring only a small part of the space
- However, [[Depth-First Search (DFS)]] may get stuck following a deep or infinite [[path(s)]] even when a [[solution(s)]] exists at a relatively shallow level
- Therefore, [[Depth-First Search (DFS)]] is not [[Complete]] and not [[Optimal]]
    - avoid [[Depth-First Search (DFS)]] for problems with deep or infinite [[path(s)]]