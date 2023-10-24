finding a plan by converting the problem into a [[Propositional Knowledge Base]] $\Phi$
- a [[satisfiable]] [[interpretation]] of $\Phi$: assign TRUE to the [[action(s)]] that are part of a correct plan; false to the others
- if there is no correct plan, $\Phi$ is not [[satisfiable]]

### Main components of [[SATPlan]]
1. [[TranslateToSAT]]
2. [[SAT solvers]]
3. [[ExtractPlan]]

>> Check the main steps of [[TranslateToSAT]](Translate a [[PDDL]] description to [[SATPlan]]) 
![[Pasted image 20231024160111.png]]
![[Pasted image 20231024160613.png]]
## Disadvantages
- [[planning]] problem usually requires a large [[Propositional Knowledge Base]]:
	- [[TranslateToSAT]] needs to create
	- $(Tmax +1) \times |Obj|^Argsp$
	- 


>conjunctive normal form not being tested

Related to: [[Satisfiability Problem (SAT)]]