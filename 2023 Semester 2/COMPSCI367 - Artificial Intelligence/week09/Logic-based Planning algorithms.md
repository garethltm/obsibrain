description language to specify [[Planning task]]
- [[Propositional Logic]]
- [[First-Order Logic]]

-  [[Propositional Logic]]-based planning
	- [[SATPlan]] ([[SAT solvers]])
-  [[Logic Programming]]-based planning
	- Prolog planner

- States can be expressed as logical sentences
- Actions can be expressed as logical rules that describe the effect (where you capture state transitions)
- Goal → this is only true if a sequence of [[action(s)]] are true which triggers a sequence of state transitions that links the [[Initial State (Start State)]] with the [[Goal(s) - Goal State(s)]]
>> [[Planning task]] can be expressed as a 
>> [[Knowledge Base (KB)]] φ (related to [[Logic Inference Problem]]) 
>> φ = [[Initial State (Start State)]] ∧ [[action(s)]] descriptions ∧ [[Goal(s) - Goal State(s)]]
>> 
>> [[2023 Semester 2/COMPSCI367 - Artificial Intelligence/week09/Planning]] is equivalent to checking the [[satisfiable]] of φ (satisfies the [[Knowledge Base (KB)]])

>	#Example 
>	finding an [[interpretation]] π such that: π ⊧ φ

![[Untitled 6.png]]
- represent the planning problem using logical [[syntax]] & extract the sequence of [[action(s)]] from there