- [[State Space]]
- [[plan]] are [[path(s)]] from [[initial state (start state)]] to [[goal(s) - goal state(s)]]

## [[planning]] vs [[search]]
>	main difference = [[state(s)]] representation
- [[planning]] 
	- [[state(s)]] (typically the [[Structured Representation]]): structural information used by [[planning]] [[algorithm]]
- [[search]]  
	- [[state(s)]] (typically the [[Atomic Representation]]): single entity used by the [[search]] [[algorithm]]
![[Untitled 5.png]]
## A planning system does:
1. Action selection based on the internal structures of [[action(s)]] & [[goal(s) - goal state(s)]] representations
2. [[subgoal]] through regression
3. [[heuristic(s)]] through relaxing preconditions

## Algorithms
1. [[Forward (Progression) planning]]
2. [[Backward (Regression) planning]]