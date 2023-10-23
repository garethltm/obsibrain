- can be used by multiple algorithms
- it mainly parses from both directions
![[Pasted image 20231023134600.png]]

## Main Idea
- idea: search both forward from the initial state and backward from the goal, and stop when the 2 searches meet in the middle
- we need an efficient way to check if a new node already appears in the other half of the search. The complexity analysis assumes this can be done in constant time, using a Hash Table
- assume branching factor = b in both directions and that there is a solution at depth = d. Then bidirectional search finds a solution in O($2b^\frac d2$) = O($b^\frac d2$) time steps.
- to check for intersection it must have all states from one of the searches in memory, therefore space complexity is O($b^\frac d2$) + O($b^\frac d2$) = 2O($b^\frac d2$) = O($b^\frac d2$)