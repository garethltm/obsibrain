- series of [[Hill-Climbing]] searches
	- (from randomly generated [[initial state (start state)]])
- overcomes local maxima
	- [[trivially complete]]

## Steps
1. Run [[Hill-Climbing]] from a random starting candidate
2. If stuck/taking too long → repeat step (1)

## Variations
1. For each restart: 
	- run until termination 
	- run for a fixed time
2. Run a fixed number of restarts
3. Run indefinitely

## Analysis
> each search has a probability p of success
> 		for 8-queens, p = 0.14 with no sideways moves
> What are the expected number of restarts? expected number of steps taken?

### Calculating the expected number of runs
-  Since, each [[try]] of [[Local Search]] starts at random
- Suppose a single [[try]] of [[greedy descent]] has a success rate of p
	- then the expected number of [[try]] needed to find the optimal solution is $\frac {1}{p}$
