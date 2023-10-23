![[Pasted image 20231023161228.png]]
- [[Constraint Satisfaction Problem (CSPs)]] can be solved by assigning values to variables one by one, in different combinations.
- Whenever a [[constraint(s)]] is violated, we go back to the most recently assigned variable & assign it a new value.
This can be achieved by a [[Depth-First Search (DFS)]] on a special kind of [[State Space]], where [[state(s)]] are defined by the values so far:
- [[initial state (start state)]]
	- the empty assignment
- [[successor function]]
- [[goal test]]

>We always go for the 1st element in the [[frontier (open list, fringe)]] because we are implementing as a [[stack]]