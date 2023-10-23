![[Pasted image 20231023161228.png]]
- [[Constraint Satisfaction Problem (CSPs)]] can be solved by assigning values to variables one by one, in different combinations.
- Whenever a [[constraint(s)]] is violated, we go back to the most recently assigned variable & assign it a new value.
This can be achieved by a [[Depth-First Search (DFS)]] on a special kind of [[State Space]], where [[state(s)]] are defined by the values so far:
- [[Initial State (Start State)]]
	- the empty assignment
- [[successor(s)]] function
	- assign a value to an unassigned variable that does not conflict with previously assigned values of other variables.
	- (If no legal values remain, the successor function fails.)
- [[Goal test]]