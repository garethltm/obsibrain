![[Pasted image 20231023170425.png]]
- can we detect this failure earlier?
## Main Idea
- Keep track of remaining legal values for unassigned variables
- Terminate search when any variable has no legal values
    - prune off that part of the [[search tree]] & backtrack

