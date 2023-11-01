- [[State Space]]
- [[plan]] are [[path(s)]] from [[initial state (start state)]] to [[goal(s) - goal state(s)]]

## [[COMPSCI367 - Artificial Intelligence/week09/Planning]] vs [[search]]
>	main difference = [[state(s)]] representation
- [[COMPSCI367 - Artificial Intelligence/week09/Planning]] 
	- [[state(s)]] (typically the [[Structured Representation]]): structural information used by [[COMPSCI367 - Artificial Intelligence/week09/Planning]] [[algorithm]]
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