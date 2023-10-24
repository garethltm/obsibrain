applying [[action(s)]] & checking whether if you are closer to the [[goal(s) - goal state(s)]]

### Action Scheme
1. `state s` → [[initial state (start state)]]
			- applicable set
			    - `Applicable(s)` = {a | a is an [[action(s)]], s ⊧ `Precond(a)`}
2. `state s` → [[initial state (start state)]]; `action a`
			- progressed state → resulting [[state(s)]] after applying `action a` at `state s`
			    - `Progress(s,a)` = (`state s` \ `Del(a)`) ∪ `Add(a)`

### Complexity Issue
1. Irrelevant [[action(s)]] → You might end up getting [[state(s)]] that are not relevant to the [[goal(s) - goal state(s)]]
2. Large search space → Taking up loads of space in [[Search]] of finding your [[goal(s) - goal state(s)]]