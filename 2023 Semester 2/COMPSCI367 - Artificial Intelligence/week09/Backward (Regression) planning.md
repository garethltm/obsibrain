start from [[Goal(s) - Goal State(s)]] & finding a sequence of steps that reaches the [[Initial State (Start State)]] by iteratively applying [[action(s)]] in the backward direction
### Action Scheme
1. `action a` is relevant to `goal g` if it satisfies **one or both** of these conditions:
    - at least 1 of `action a` ’s effects (can be + or -) unifies with an element of `goal g`
    - none of `action a` ‘s effects (can be + or -) negates an element of `goal g`
	    
	    <aside> 💡 as long as there is an effect that doesn’t go away from the goal</aside>
    - In this case, we write `action a` ∈ `Relevant(g)`
    
2. regressed [[subgoal]] → from `goal g` over `action a` is:
    - `Regress(g,a)` = (`goal g` \ `Add(a)`) ∪ `Precond(a)`

		<aside> 💡 Backward planning can be more effective in certain context</aside>![[Pasted image 20231024154602.png]]

### Advantages
generally reduced [[branching factor(s)]]. Suitable for cases when there is a large number of ground [[action(s)]]
>	#Example 
>	![[Pasted image 20231024154715.png]]