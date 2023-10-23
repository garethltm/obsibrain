![[Pasted image 20231023170425.png]]
- can we detect this failure earlier?
## Main Idea
- Keep track of remaining legal values for unassigned variables
- Terminate search when any variable has no legal values
    - prune off that part of the [[search tree]] & backtrack

### Constraint Propagation
- Forwards checking propagates information from assigned to unassigned variables, but doesn’t provide early detection for all failures:![[Pasted image 20231023170515.png]]![[Pasted image 20231023170532.png]]
- Idea of the algorithm is to keep track of all domains for every variable & take the values out