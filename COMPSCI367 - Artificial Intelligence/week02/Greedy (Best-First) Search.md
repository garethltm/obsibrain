![[Pasted image 20231023145952.png]]

## Main Idea
- select the [[path(s)]] whose end is closest to a [[Goal(s) - Goal State(s)]] according to the [[heuristic(s)]] function
    
- Greedy Best-First Search - Best-First Search selects the next node for expansion using the heuristic function for its evaluation function, ie. f(n) = h(n)
    
    - h(n)=0 → n is a goal state
    
    > Example: greedy search **minimises the estimated cost to the goal**; it expands whichever node n is estimated to be closest to the goal
    
- It treats the frontier as a priority queue ordered by h