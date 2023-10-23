- Often, we are not given an algorithm to solve a problem, but only a specification of a [[solution(s)]].
	> which means we have to search for it
	- Typical problems
		- [[agent]] is in "[[Initial State (Start State)]]" where it has a set of [[Deterministic]] [[action(s)]] it can carry out & wants to get to [[goal(s) - goal state(s)]]
	- Many AI problems can be abstracted into the problem of finding a [[path(s)]] in a [[Directed Graph]]
- There is usually more than one way to represent a problem as a Graph
1. [[Uninformed Search]] can only distinguish between [[goal(s) - goal state(s)]] & non-[[goal(s) - goal state(s)]] 
2. [[Informed Search]] uses [[heuristic(s)]] to try to get "closer" to the [[goal(s) - goal state(s)]]