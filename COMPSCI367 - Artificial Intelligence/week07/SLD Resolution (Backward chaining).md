- iteratively replace goals with subgoals; try to get head with an empty body

## Main Idea
- `yes ← g`, then you keep going backwards from g adding stuff to it to eventually reach to a state where; `yes ←`
    - G (a set which contains whatever the current state is) - G will increase up to a certain point, then it will start to decrease where it would eventually reach 0

#### Problem with SLD:
- **No mechanism for backtracking purposes**
    - You might end up searching through the entire [[search tree]], which would eventually mean that it isn’t much different than **[[Forward Chaining]]**
    - Theoretically it would still mean that it is not efficient but in practice it is still more efficient because of the [[Backtracking Search]] idea
- **[[Soundness]]** → search procedure is success (it derives goal), we can then work [[Backtracking Search]] & turn it into a forward chaining proof
- **Completeness** → because of the completeness of forward chaining, SLD resolution is also complete
    - we need to use a complete search method that will not go into an infinite path
        
        > BFS, Iterative Deepening Search, etc.