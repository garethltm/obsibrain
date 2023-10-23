![[Pasted image 20231022160231.png]]
- Randomly generated 8-queens [[Start States]]
	- Get stuck 86% of the time
	- Solves only 14% of problem instances
> Sometimes, 
> 1. in [[Depth-First Search (DFS)]] we might get into a situation where we can get stuck (no solution). 
> 2. in [[Greedy (Best-First) Search]] we might be looking for the best [[heuristic(s)]] value at every [[state]] which might end up in a dead node
> We use [[Hill-Climbing]] to see whether if it gets stuck

#### Why is it not that BAD
- 4 steps on average when it succeeds
	> Applying Backtracking 8-Queens → we need to make at least 8 assignments (for every depth = 1 assignment)
	> - which in this case we are already saving quite a bit of steps
- 3 steps on average when it gets stuck
- [[state space]] with $8^8$ = ~17 million [[state(s)]]
