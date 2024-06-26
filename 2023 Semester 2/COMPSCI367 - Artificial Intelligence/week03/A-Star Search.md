**[[Uniform-Cost Search (UCS) (Lowest-Cost-First Search)]]** 
- orders by [[path cost]] or backward cost: **g(n)**
**[[Greedy (Best-First) Search]]** 
- orders by **goal proximity** or forward cost: **h(n)**
*A-Star Search orders by the sum:* f(n) = **g(n)** + **h(n)**
- Order [[Priority Queue]] using function **f(n)** = **g(n)** + **h(n)**

[[Uniform-Cost Search (UCS) (Lowest-Cost-First Search)]] minimizes **g(n)**
- [[Optimal]] & [[Complete]] but not efficient
[[Greedy (Best-First) Search]] minimizes **h(n)**
- efficient but not [[Optimal]] or [[Complete]]
![[Pasted image 20231023150701.png]]
- combination of both [[Uniform-Cost Search (UCS) (Lowest-Cost-First Search)]] & [[Greedy (Best-First) Search]]
### Additional Information
- preserve efficiency of [[Greedy (Best-First) Search]] but avoid expanding [[path(s)]] that are already expensive
### Heuristic Function
![[Pasted image 20231023151300.png]]
**Heuristic estimate f(n)** of the cost of the cheapest paths from s to t via n:
**f(n)** = **g(n)** + **h(n)**
- **g(n)** is the ==**cost of an optimal path**== from s to n
- **h(n)** is an ==**estimate of the cost of an [[Optimal]] path**== from n to t

#### Is [[A-Star Search]] [[Optimal]] & [[Complete]]?
- Yes, provided h(n) is [[Admissible heuristic]] 

##### Conditions for [[Optimal]]
	 $∀n\ h(n) ≤ y(n)$
		- where y(n) is the true cost from n to the [[goal(s) - goal state(s)]]
	- If ***h(n)*** is [[Admissible heuristic]] then **f(n)** **never overestimates** the actual cost of the best solution through n
	- Theorem: [[A-Star Search]] finds optimal solution if **h(n)** is [[Admissible heuristic]]

Hence, the theorem:
**_If h(n) is [[Consistent heuristic]], [[A-Star Search]] is [[Optimal]]***

### A-Star Graph Search gone WRONG
![[Pasted image 20231023155524.png]]

### A* - What to do if h is NOT CONSISTENT
- So far, we have assumed that h is [[Consistent heuristic]] (thus [[Admissible heuristic]]); but what if h is not [[Consistent heuristic]] (but still [[Admissible heuristic]])
- If **h is not consistent** then we have **no guarantee** that the 1st time **[[State(s)]] s** is picked to be expanded that its **cheapest path from i has been found**
- This means that if s is already in the [[closed list]], a cheaper [[path(s)]] may be found & this new [[path(s)]] will need to “replace” the old one
	- if we meet that [[State(s)]] again & the evaluation value is smaller then you will need to reopen
## Properties
- [[Complete]]
    - Yes, unless there are infinitely many nodes with f ≤ cost of solution
- [[Time Complexity]]
    - $O(b^d)$ 
- [[Space Complexity]]
    - $O(b^d)$ - Keeps all nodes in memory
- [[Optimal]]
    - Yes (assuming h is [[Admissible heuristic]])

## Summary:
- [[A-Star Search]] uses both backward cost g & (estimates of) forward costs h
- [[A-Star Search]] is [[Optimal]] with [[Admissible heuristic]]/[[Consistent heuristic]]
- [[heuristic(s)]] design is key: often use relaxed problems