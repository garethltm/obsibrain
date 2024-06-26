### Summary
- tries to minimise [[path cost]] from current node n to [[Goal(s) - Goal State(s)]]

### Additional Information
- select the [[path(s)]] whose end is closest to a [[Goal(s) - Goal State(s)]] according to the [[heuristic(s)]] function
- selects the next node for expansion using the [[heuristic(s)]] function for its evaluation function, ie. `f(n) = h(n)`
    - `h(n)=0` → n is a [[Goal(s) - Goal State(s)]]
>	#Example 
>	[[Greedy (Best-First) Search]] **minimises the estimated cost to the [[goal(s) - goal state(s)]]**; it expands whichever node n is estimated to be closest to the [[goal(s) - goal state(s)]]
- It treats the [[frontier (open list, fringe)]] as a [[Priority Queue]] ordered by [[heuristic(s)]]
- find [[Goal(s) - Goal State(s)]] quickly but not necessarily the optimal one
![[Pasted image 20231023145952.png]]
## Properties
- [[Complete]]
	- generally no! can get stuck in loops
>	#Example 
>	but [[complete]] in finite space with repeated-state checking
- [[Time Complexity]]
	- $O(b^m)$, where m is the maximum depth in search space
- [[Space Complexity]]
	- $O(b^m)$ (retains all nodes in memory)
- [[Optimal]]
	- No!

>[[Greedy (Best-First) Search]] has the same time deficits as [[Depth-First Search (DFS)]]. 
>However, a good [[heuristic(s)]] can reduce [[Time Complexity]] and [[Space Complexity]] costs substantially.