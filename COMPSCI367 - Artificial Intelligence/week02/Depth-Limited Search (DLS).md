- solves the infinite loop **problem**

## Properties
- [[COMPSCI367 - Artificial Intelligence/week02/Complete]]
    - Yes - no infinite loops anymore
	- Even if there is loops in the graph, it can’t go infinitely as it would cycle within the limit of the maximum number of steps but will still need to go back and traverse to other parts of the graph
- [[Time Complexity]]
    - $O(b^k)$ 
	    - where k is the depth limit
- [[Space Complexity]]
    - $O(bk)$ 
	    - linear space similar to [[Depth-First Search (DFS)]]
- [[Optimal]]
    - No, can find [[suboptimal]] [[solution(s)]] first
	1. If u set the limit at the level of the [[solution(s)]] 
		- it is supposed to find it at the shallowest level. 
	2. If your depth limit is higher than the depth of the [[solution(s)]]
		- it might take extra steps to arrive to the [[solution(s)]]
	![[Pasted image 20231022040347.png]]

>Expands nodes like [[Depth-First Search (DFS)]] but imposes a cutoff on the maximum depth of [[path(s)]]