- Also known as [[iterative improvement]]
- [[frontier (open list, fringe)]] maintains some unexpanded successors of expanded nodes
- Start from some [[state(s)]] & "move" from present location(s) to neighbouring location(s). 
	- These moves are determined by the present location(s).
- Not guaranteed to be [[complete]]
- [[Single-agent]] environment
- solve large complex search problems with small memory
	- small memory because you only need to know the [[current state]]
	- maintains & iteratively updates a single [[candidate solution]]

In many optimisation problems:
- [[path(s)]] is irrelevant
- [[goal(s) - goal state(s)]] is the solution
- [[State Space]] = set of "complete" configuration
	![[Pasted image 20231022173408.png]]
	1. find configuration satisfying constraints
		> n-queens problem
	2. find optimal configuration
		>travelling salesperson problem
	>- We can use [[Iterative Improvement]] algorithms to keep a single "current" state, try to improve it
	>- Constant space, suitable for online as well as offline search

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
- General familie