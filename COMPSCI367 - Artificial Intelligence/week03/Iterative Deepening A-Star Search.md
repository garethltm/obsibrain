[[Iterative Deepening A-Star Search]] is a low-memory variant of [[A-Star Search]] which performs a series of [[Depth-First Search (DFS)]] but cuts off each search when the sum 
- f() = g() + h() exceeds some pre-defined threshold

The threshold is steadily increased with each successive search. It starts at the estimate of the cost at the [[Initial State (Start State)]], and increases for each iteration of the algorithm. At each iteration, the threshold used for the next iteration is the minimum cost of all values that exceeded the current threshold

[[Iterative Deepening A-Star Search]] is asymptotically as efficient as [[A-Star Search]] for domains where the number of states grow exponentially

>The limit is set not by depth but their evaluation value

## Properties
- [[Complete]]
	- Yes
	    - unless there are infinitely many nodes with $f ≤ cost\ of\ solution$
- [[Time Complexity]]
	-  $O(b^d)$
- [[Space Complexity]] (similar to [[Depth-First Search (DFS)]])
	- $O(bd)$ 
		- it need only store a stack of nodes which represents the branch of the tree it is expanding
- [[Optimal]]
	- Yes (assuming $h(n)$ is [[Admissible heuristic]])

### Is IDA* better than A*
Short answer:
- [[Space Complexity]] wise ✅
- [[Time Complexity]] sometimes
Long answer:
- [[a]] uses priority queue, IDA_ uses a stack**
- IDA* doesn’t need to deal with neither open or closed lists, but A* does
- Runtime will depend on how frequently duplicate states will be encountered and iterations are done
- If you don’t have much memory, but can wait for the solution - use IDA*