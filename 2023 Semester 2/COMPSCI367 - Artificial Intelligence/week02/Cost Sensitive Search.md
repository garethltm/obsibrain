- [[Depth-First Search (DFS)]] is not [[Optimal]]
- [[Breadth-First Search (BFS)]] finds the shortest [[path(s)]] in terms of number of [[action(s)]]. It does not find the least-cost [[path(s)]]

![[Pasted image 20231023140110.png]]
- [[Uniform-Cost Search (UCS) (Lowest-Cost-First Search)]] is similar to [[Breadth-First Search (BFS)]], but sorts the [[Queue]] using the [[path(s)]] cost
    - Expands the lowest [[path(s)]] cost
    ### Good
	-  [[Uniform-Cost Search (UCS) (Lowest-Cost-First Search)]] is [[Complete]] and [[Optimal]]
    ### Bad
	- explores options in every “direction”
    - No information about the [[Goal(s) - Goal State(s)]] location
    ![[Pasted image 20231023140125.png]]
    - doesn't know where to go
    - the blue node would be the optimal path; [[Uniform-Cost Search (UCS) (Lowest-Cost-First Search)]] would prioritise the black nodes instead which is not [[Optimal]]