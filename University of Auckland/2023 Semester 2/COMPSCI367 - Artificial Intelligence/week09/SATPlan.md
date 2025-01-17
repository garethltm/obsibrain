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
- [[University of Auckland/2023 Semester 2/COMPSCI367 - Artificial Intelligence/week09/Planning]] problem usually requires a large [[Propositional Knowledge Base]]:
	- [[TranslateToSAT]] needs to create
	- $(Tmax +1) \times |Obj|^{Argsp}$
		- for new [[Atomic Propositions (atoms)]] for each predicate symbol
	- $(Tmax +1) \times |Obj|^{Argsp}$
		- for new [[Atomic Propositions (atoms)]] for each action schema
	- where $|Obj|$ is the set of constants, $Args\tiny p$ is the maximum arity of a predicate, $Args\tiny A$ is the maximum arity of an action scheme

## Advantages
Speed
- Utilising efficient [[domain-independent heuristic]] for [[Propositional Logic]] reasoning
- Taking advantage of mature [[SAT solvers]] such as DPLL, which is highly optimised
- Fixed structure in [[Classical Planning]] domain & problem means that further optimisation is possible

>conjunctive normal form not being tested

Related to: [[Satisfiability Problem (SAT)]]