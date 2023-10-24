start from [[goal(s) - goal state(s)]] & checking whether you reach the [[initial state (start state)]]

### Action Scheme
1. `action a` is relevant to `goal g` if it satisfies **one or both** of these conditions:
    - at least 1 of `action a` ’s effects (can be + or -) unifies with an element of `goal g`
    - none of `action a` ‘s effects (can be + or -) negates an element of `goal g`
	    
	    <aside> 💡 as long as there is an effect that doesn’t go away from the goal</aside>
    - In this case, we write `action a` ∈ `Relevant(g)`
    
2. regressed subgoal → from `goal g` over `action a` is:
    - `Regress(g,a)` = (`goal g` \ `Add(a)`) ∪ `Precond(a)`

		<aside> 💡 Backward planning can be more effective in certain context
		</aside>