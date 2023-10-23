- Often, we are not given an algorithm to solve a problem, but only a specification of a [[solution(s)]].
	> which means we have to search for it
	- Typical problems
		- [[Agent]] is in "[[Initial State (Start State)]]" where it has a set of [[Deterministic]] [[action(s)]] it can carry out & wants to get to [[Goal(s) - Goal State(s)]]
	- Many AI problems can be abstracted into the problem of finding a path in a [[Directed Graph]]
- There is usually more than one way to represent a problem as a Graph
1. [[Uninformed Search]] can only distinguish between [[Goal(s) - Goal State(s)]] & non-[[Goal(s) - Goal State(s)]] 
2. [[Informed Search]] uses [[Heuristics]] to try to get "closer" to the [[Goal(s) - Goal State(s)]]