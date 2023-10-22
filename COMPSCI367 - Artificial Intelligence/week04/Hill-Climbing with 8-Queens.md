- Randomly generated 8-queens Start States
	- Get stuck 86% of the time
	- Solves only 14% of problem instances
> Sometimes, in [[Depth-First Search (DFS)]] we might get into a situation where we can get stuck (no solution)
> We use [[Hill-Climbing Search]] to see whether if it gets stuck


#### Why is it not that BAD
- 4 steps on average when it succeeds
- 3 steps on average when it gets stuck
	- State Space with $8^8$ = ~17 million states