[[Iterative Deepening A-Star Search]] is a low-memory variant of [[A-Star Search]] which performs a series of [[Depth-First Search (DFS)]] but cuts off each search when the sum 
- f() = g() + h() exceeds some pre-defined threshold

The threshold is steadily increased with each successive search. It starts at the estimate of the cost at the [[Initial State (Start State)]], and increases for each iteration of the algorithm. At each iteration, the threshold used for the next iteration is the minimum cost of all values that exceeded the current threshold

[[Iterative Deepening A-Star Search]] is asymptotically as efficient as [[A-Star Search]] for domains where the number of states grow exponentially

>