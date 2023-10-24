- problem solving
- possibilities of just moving from one [[state(s)]] to another [[state(s)]]

1. [[Forward Planning]]
	- ### Action Scheme
		1. `state s` → initial state/start state
			- applicable set
			    - `Applicable(s)` = {a | a is an action, s ⊧ `Precond(a)`}
		2. `state s` → initial state/start state; `action a`
			- progressed state → resulting state after applying `action a` at `state s`
			    - `Progress(s,a)` = (`state s` \ `Del(a)`) ∪ `Add(a)`