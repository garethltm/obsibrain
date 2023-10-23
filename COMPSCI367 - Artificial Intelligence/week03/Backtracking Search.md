![[Pasted image 20231023161228.png]]
- [[Constraint Satisfaction Problem (CSPs)]] can be solved by assigning values to variables one by one, in different combinations.
- Whenever a [[constraint(s)]] is violated, we go back to the most recently assigned variable & assign it a new value.
This can be achieved by a [[Depth-First Search (DFS)]] on a special kind of [[State Space]], where [[state(s)]] are defined by the values so far:
- [[initial state (start state)]]
	- the empty assignment
- [[successor function]]
- [[goal test]]

>We always go for the 1st element in the [[frontier (open list, fringe)]] because we are implementing as a [[stack]]

### Properties
The search space for this [[Depth-First Search (DFS)]] has certain very specific properties:
- **If there are n variables, every [[solution(s)]] will occur at exactly depth n**
- Variable assignments are commutative
    > Example: [**WA = red** then **NT = green**] same as [**NT = green** then **WA = red**]

> [[Breadth-First Search (BFS)]] is bad because of the possible [[branching factor(s)]] due to the number of variables which is equivalent to the depth which may take really long

### Improvements to Backtracking Search
General-purpose methods can give huge gains in speed:
1. Which variable should be assigned next?
2. In what order should its values be tried?
3. Can we detect inevitable failure early?