- simplest [[Search Techniques (Search Strategy) (Search Algorithm)]] that is guaranteed to find a minimum [[path cost]]
	- similar to [[Breadth-First Search (BFS)]] but it selects a [[path(s)]] with the ==lowest cost==
	- the [[frontier (open list, fringe)]] is implemented as a [[Priority Queue]] ordered by the ==cost function==

**Sometimes there are cost associated with [[arc]]. The cost of a [[path(s)]] is the sum of the cost of its [[arc]]**
- an optimal [[solution(s)]] is one with minimum cost
- for many domains, [[arc]] have non-unit costs, the aim is to find an optimal [[solution(s)]], a [[solution(s)]] such that no other [[solution(s)]] has a lower total cost

## Steps
 Implementation: [[priority queue]] = insert nodes in order of increasing [[path cost]]
	(`lowest path cost g(n)`)
1. Expand root first, 
2. Expand least-cost unexpanded node
3. Reduces to [[Breadth-First Search (BFS)]] when all [[action(s)]] have same cost
4. Finds the cheapest goal provided [[path cost]] is monotonically increasing along each [[path(s)]] 
> (no negative-cost steps)
> Also, sorting whenever we add a node

## Properties
1. [[Complete]]
	- Yes, if b is finite & if step cost ≥ ε with ε > 0
2. [[Time Complexity]]
	- $O(b^[1+\frac C ε])$ 
		- where C* = cost of the optimal [[solution(s)]]
		- assume every [[action(s)]] costs at least ε, where ε is the least cost [[action(s)]]
3. [[Space Complexity]] - we need to store all the nodes we want to explore
	-  $O(b^[1+\frac C ε])$
		- number will depend on that minimum cost associated to an [[arc]] to that ε
		- smaller the ε means more nodes we might need to store in our [[frontier (open list, fringe)]]
4. [[Optimal]]
	- Yes, if nodes expanded in increasing order of `g(n)`![[Pasted image 20231022030918.png]]
> ε (epsilon) - least-cost [[action(s)]] 
> C - cost of the optimal [[solution(s)]]
> $\frac Cε$ would represent the number of steps that might be required to find the [[goal(s) - goal state(s)]]. 
> 
> In other words, approximates the depth at which the [[solution(s)]] can be found. 
> 
> The computation of the time/[[space complexity]] in this case would be similar to [[Breadth-First Search (BFS)]] $O(b^d)$ 
> - b - [[branching factor(s)]]
> - d - depth of the [[solution(s)]]]

Worst case scenario: we will need to visit all the nodes stored in the [[frontier (open list, fringe)]]; which means that the [[Time Complexity]] = [[Space Complexity]]