### Summary
- returns a [[solution(s)]]
	- doesn't maintain a path ("only a current [[state(s)]]")
- Many [[Constraint Satisfaction Problem (CSPs)]] can be formulated as [[Local Search]]
- General families of algorithms:
	- [[Local Search]] + [[Gradient descent]]
		- [[Hill-Climbing]]
		- [[Hill-Climbing with side-way moves]]
		- [[Tabu Search]]
		- [[Enforced Hill-Climbing]]
	- [[Stochastic Search]]
	- [[Population-based Search]]
> Many machine learning algorithms are [[Local Search]]

### Additional Information
- Also known as [[iterative improvement]]
- [[frontier (open list, fringe)]] maintains some unexpanded [[successor(s)]] of expanded nodes
- Start from some [[state(s)]] & "move" from present location(s) to neighbouring location(s). 
	- These moves are determined by the present location(s).
- Not guaranteed to be [[complete]]
	- can go from 1 neighbour to another then get stuck
- [[Single-agent]] environment
- designed to solve large complex search problems with small memory ([[Space Complexity]])
	- small memory because you only need to know the [[current state]]
	- maintains & iteratively updates a single [[candidate solution]]

In many optimisation problems:
- [[path(s)]] is irrelevant
- [[goal(s) - goal state(s)]] is the [[solution(s)]]
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
		- cannot have a "complete [[goal(s) - goal state(s)]]" because the problem will already be solved
- number of runs
	- specify when to stop
		- Travelling Salesperson Problem

## Steps
1. we start from some [[initial state (start state)]]
2. perform a number of [[action(s)]] searching for a [[solution(s)]]

## Main Idea
- resembling an [[agent(s)]] exploring the search space & move along [[successor(s)]] relations
	- AIM: to improve its position in the long run (optimal solution)

## Problem
- could lead to a [[path(s)]] without an [[optimal]] solution