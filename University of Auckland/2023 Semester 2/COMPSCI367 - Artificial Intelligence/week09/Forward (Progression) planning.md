applying [[action(s)]] & checking whether if you are closer to the [[Goal(s) - Goal State(s)]]

### Action Scheme
1. `state s` → [[Initial State (Start State)]]
			- applicable set
			    - `Applicable(s)` = {a | a is an [[action(s)]], s ⊧ `Precond(a)`}
2. `state s` → [[Initial State (Start State)]]; `action a`
			- progressed state → resulting [[State(s)]] after applying `action a` at `state s`
			    - `Progress(s,a)` = (`state s` \ `Del(a)`) ∪ `Add(a)`
![[Pasted image 20231024154243.png]]
### Complexity Issue
1. Irrelevant [[action(s)]] → You might end up getting [[State(s)]] that are not relevant to the [[Goal(s) - Goal State(s)]]
>	#Example 
>	![[Pasted image 20231024154304.png]]
1. Large search space → Taking up loads of space in [[Search]] of finding your [[Goal(s) - Goal State(s)]]
>	#Example 
>	![[Pasted image 20231024154323.png]]