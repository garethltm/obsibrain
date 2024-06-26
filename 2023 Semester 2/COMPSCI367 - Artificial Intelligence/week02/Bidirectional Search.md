- can be used by multiple algorithms
- it mainly parses from both directions
![[Pasted image 20231023134600.png]]

## Main Idea
- search both forward from the [[Initial State (Start State)]] and backward from the [[Goal(s) - Goal State(s)]], and stop when the 2 searches meet in the middle
- we need an efficient way to check if a new node already appears in the other half of the search. The complexity analysis assumes this can be done in ==constant time==, using a Hash Table
	- assume [[branching factor(s)]] = b in both directions
	- assume there is a solution at depth = d. 
	- Then bidirectional search finds a solution in O($2b^\frac d2$) = O($b^\frac d2$) time steps.
- to check for intersection it must have all [[State(s)]] from one of the searches in memory, therefore [[Space Complexity]] is O($b^\frac d2$) + O($b^\frac d2$) = 2O($b^\frac d2$) = O($b^\frac d2$)

## Properties
- [[Complete]]
    - Depends on the search algorithm used. If [[Breadth-First Search (BFS)]], then yes
- [[Time Complexity]]
    - $O(b^\frac d2)$
- [[Space Complexity]]
    -  $O(b^\frac d2)$
- [[Optimal]]
    - Depends on the [[Search Techniques (Search Strategy) (Search Algorithm)]] used

>Bidirectional search is [[Uninformed Search]] strategy as it only uses the information provided by the [[State Space]]. 
>
>For [[State Space Problem]], we assume that the location of the [[Goal(s) - Goal State(s)]] is known to the [[agent(s)]]. The [[solution(s)]] of the search is not the location of the [[Goal(s) - Goal State(s)]], but the [[path(s)]] to the [[Goal(s) - Goal State(s)]].