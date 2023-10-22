- Often, we are not given an algorithm to solve a problem, but only a specification of a [[Solution]].
	> which means we have to search for it
	- Typical problems
		- [[Agent]] is in "initial [[State]]" where it has a set of [[Deterministic]] [[Action]] it can carry out & wants to get to [[Goal]] state
	- Many AI problems can be abstracted into the problem of finding a path in a [[Directed Graph]]
- There is usually more than one way to represent a problem as a Graph
1. [[Uninformed Search]] can only distinguish between [[Goal]] states & non-[[Goal]] states
2. [[Informed Search]] uses [[Heuristics]] to try to get "closer" to the [[Goal]]