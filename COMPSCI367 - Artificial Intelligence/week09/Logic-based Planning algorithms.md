-  [[Propositional Logic]]-based planning
	- SATPlan ([[SAT solvers]])
-  [[Logic Programming]]-based planning
	- Prolog planner

- States → logical sentences

- Actions → logical rules that describe the effect (where you capture state transitions)

- Goal → this is only true if a sequence of actions are true which triggers a sequence of state transitions that links the initial state with the goal

>> Planning task can be expressed as a [[Knowledge Base (KB)]] φ (related to logical inference) φ = initial state ∧ action descriptions ∧ goal
>> 
>> Planning is equivalent to checking the satisfiability of φ (satisfies the KB)
>>>Example: finding an interpretation π such that: π ⊧ φ

![[Untitled 6.png]]
- represent the planning problem using logical syntax & extract the sequence of actions from there