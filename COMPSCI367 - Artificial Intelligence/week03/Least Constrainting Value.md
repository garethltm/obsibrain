- given a variable, choose the least constraining value:
	- the one that rules out the fewest values in the remaining variables

![[Pasted image 20231023163245.png]]
1. we pick WA first then we pick Q next. Where Q has 3 legal values it can pick from
2. if G = green/blue; NT & SA now only have 1 legal value to only pick from
3. if G = red; NT & SA can have 2 legal values to pick from

- more generally, 3 allowed values would be better than 2, etc.
	- combining these heuristics makes multi-variable CSP with big domains feasible