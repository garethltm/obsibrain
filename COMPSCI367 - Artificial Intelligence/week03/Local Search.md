- Also known as [[iterative improvement]]
- [[frontier (open list, fringe)]] maintains some unexpanded successors of expanded nodes
- Start from some [[state(s)]] & "move" from present location(s) to neighbouring location(s). 
	- These moves are determined by the present location(s).
- Not guaranteed to be [[COMPSCI367 - Artificial Intelligence/week02/Complete]]
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
	>- We can use [[Iterative Improvement]] algorithms to keep a single "current" state, try to improve it
	>- Constant space, suitable for online as well as offline search

## Algorithms
- [[Hill-Climbing]]

## Steps
1. we start from some [[initial state (start state)]]
2. perform a number of [[action(s)]] searching for a [[solution(s)]]

## Main Idea
- resembling an [[agent]] exploring the search space & move along successor relations
	- AIM: to improve its position in the long run (optimal solution)

## Problem
- could lead to a [[path(s)]] without an [[optimal]] solution

### Summary
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