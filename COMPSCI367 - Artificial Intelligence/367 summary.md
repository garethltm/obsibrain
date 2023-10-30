# Systematic Search
### Types of Uninformed Search
- [[Breadth-First Search (BFS)]]
- [[Uniform-Cost Search (UCS) (Lowest-Cost-First Search)]]
- [[Depth-First Search (DFS)]]
- [[Depth-Limited Search (DLS)]]
- [[Iterative-Deepening Search (IDS)]]
- [[Bidirectional Search]]
### Types of Informed Search
- [[Greedy (Best-First) Search]]
- [[A-Star Search]]
- [[Iterative Deepening A-Star Search (IDA)]]

# Local Search
## Constraint Satisfaction Problems
1. [[Backtracking Search]] 
	- [[Minimum Remaining Values (MRV)]]
	- [[Least Constraining Value]]
	- [[Forward Checking]]
	- [[Variable Elimination]]

- Many configuration & optimisation problems ([[Constraint Satisfaction Problem (CSPs)]]) can be formulated as [[Local Search]]
- General families of [[algorithm]]:
	- [[Local Search]] + [[Gradient descent]]
		- [[Hill-Climbing]]
		- [[Hill-Climbing with side-way moves]]
		- [[Tabu Search]]
		- [[Enforced Hill-Climbing]]
	- [[Stochastic Local Search (SLS)]]
		- [[First Choice Hill-Climbing]]
		- [[Stochastic Hill-Climbing]]
		- [[Random Walk Hill-Climbing]]
		- [[Random-Restart Hill Climbing]]
		- [[Simulated Annealing]]
> Many machine learning algorithms are [[Local Search]]- 

## Population-based Search
- [[Population-based Search]] conducts search by maintaining & updating a collection of [[candidate solution]]
- [[Local beam Search]] is an adaptation of [[Iterative Best Improvement (IBI)]] by maintaining M > 1 [[candidate solution]]
- [[Stochastic Beam Search (SBS)]] aims to avoid [[Local beam Search]] concentration on a narrow [[path(s)]] by using [[Boltzmann distribution]]

## Genetic Algorithm
- a variation of [[Stochastic Beam Search (SBS)]] that generates every [[successor(s)]] using 2 [[candidate solution]]
- to apply the [[evolution]] paradigm as a [[Search Techniques (Search Strategy) (Search Algorithm)]], we need:
	1. [[candidate solution]] representation: 
		- the most common representation of a [[candidate solution]] in S (where S is our search space) is [[chromosomes]]
	2. [[fitness]]
	3. [[crossover operation]] & [[mutation operation]]
		- these are for generating offsprings