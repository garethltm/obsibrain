### Summary
- returns a [[solution(s)]]
	- doesn't maintain a path ("only a current [[State(s)]]")
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
	- [[Population-based Search]]
> Many machine learning algorithms are [[Local Search]]

### Additional Information
- Also known as [[Iterative Improvement]]
- [[frontier (open list, fringe)]] maintains some unexpanded [[successor(s)]] of expanded nodes
- Start from some [[State(s)]] & "move" from present location(s) to neighbouring location(s). 
	- These moves are determined by the present location(s).
- Not guaranteed to be [[Complete]]
	- can go from 1 neighbour to another then get stuck
- [[Single-agent]] environment
- designed to solve large complex search problems with small memory ([[Space Complexity]])
	- small memory because you only need to know the [[current state]]
	- maintains & iteratively updates a single [[candidate solution]]

In many optimisation problems:
- [[path(s)]] is irrelevant
- [[Goal(s) - Goal State(s)]] is the [[solution(s)]]
- [[State Space]] = set of "complete" configuration
	![[Pasted image 20231022173408.png]]
	1. find configuration satisfying constraints
		> n-queens problem
	2. find optimal configuration
		>travelling salesperson problem
	>- We can use [[Iterative Improvement]] [[algorithm]] to keep a single "current" state, try to improve it
	>- Constant space, suitable for online as well as offline search

## Stopping Criteria
- [[heuristic(s)]]
	- you can use the [[heuristic(s)]] value as a termination test in some problems
		- n-queens
- [[Goal test]] 
	- you can use a [[Goal test]] like in [[Systematic Search]].
		- this will work in sudoku or n-queens
		- cannot have a "complete [[Goal(s) - Goal State(s)]]" because the problem will already be solved
- number of runs
	- specify when to stop
		- Travelling Salesperson Problem
## [[heuristic(s)]] 
- this allows the algorithm to make moves maximising or minimising the value
	- doesn't have to be [[Admissible heuristic]] or [[Consistent heuristic]]
- can be involved in the [[Goal test]] or termination condition or not

## Steps
1. we start from some [[Initial State (Start State)]]
2. perform a number of [[action(s)]] searching for a [[solution(s)]]

## Main Idea
- resembling an [[agent(s)]] exploring the search space & move along [[successor(s)]] relations
	- AIM: to improve its position in the long run (optimal solution)

## Problem
- could lead to a [[path(s)]] without an [[Optimal]] solution