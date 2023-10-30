- Feeding this [[Propositional Knowledge Base]] from ([[TranslateToSAT]]) to a [[SAT solvers]]:
	- if the [[sentence(s)]] is unsatisfiable, then there is not a valid plan
	- if a [[satisfiable]] [[interpretation]] is found, then the [[goal(s) - goal state(s)]] can be achieved (Overall conjunction)
>	#Example 
>	![[Pasted image 20231024155646.png]]
### Efficient implementations
- [[DPLL algorithm]]
- [[Local Search]] - use the number of unsatisfied [[clause(s)]] as the evaluation function
	- [[Greedy Descent]]
	- [[Simulated Annealing]]
	- WalkSAT

Related to: [[Satisfiability Problem (SAT)]] 