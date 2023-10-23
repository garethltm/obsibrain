![[Pasted image 20231023145952.png]]

## Main Idea
- select the [[path(s)]] whose end is closest to a [[Goal(s) - Goal State(s)]] according to the [[heuristic(s)]] function
- selects the next node for expansion using the [[heuristic(s)]] function for its evaluation function, ie. `f(n) = h(n)`
    - `h(n)=0` → n is a [[Goal(s) - Goal State(s)]]
    > Example: greedy search **minimises the estimated cost to the [[Goal(s) - Goal State(s)]]**; it expands whichever node n is estimated to be closest to the [[Goal(s) - Goal State(s)]]
- It treats the [[frontier (open list, fringe)]] as a [[priority queue]] ordered by h

## Properties
- [[Complete]] 
	- generally no! can get stuck in loops
    > Example: but complete in finite space with repeated-state checking
- [[Time Complexity]]
	- $O(b^m)$, where m is the maximum depth in search space
- [[Space Complexity]]
	- $O(b^m)$ (retains all nodes in memory)
- [[Optimal]]
	- No!

>Greedy Search has the same time deficits as [[Depth-First Search (DFS)]]. 
>However, a good [[heuristic(s)]] can reduce [[Time Complexity]] and [[Space Complexity]] costs substantially.