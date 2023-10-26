- Selective Linear [[Definite clause]]
- iteratively replace [[Goal(s) - Goal State(s)]] with subgoals; try to get head with an empty body
- [[SLD Resolution (Backward chaining)]] can be performed using a [[Search Techniques (Search Strategy) (Search Algorithm)]]
![[Pasted image 20231024005327.png]]
## Main Idea
- `yes ← g`, then you keep going backwards from g adding stuff to it to eventually reach to a state where; `yes ←`
    - G (a set which contains whatever the current state is) - G will increase up to a certain point, then it will start to decrease where it would eventually reach 0

![[Pasted image 20231024010154.png]]
#### Problem with SLD:
- **No mechanism for backtracking purposes**
    - You might end up searching through the entire [[search tree]], which would eventually mean that it isn’t much different than **[[Forward Chaining]]**
    - Theoretically it would still mean that it is not efficient but in practice it is still more efficient because of the [[Backtracking Search]] idea
>	#Example 
>	![[Pasted image 20231024010214.png]]

- **[[Soundness]]** → search procedure is success (it derives goal), we can then work [[Backtracking Search]] & turn it into a [[forward chaining]] proof
- **[[Completeness]]** → because of the completeness of [[forward chaining]], [[SLD Resolution (Backward chaining)]] is also [[Completeness]]
    - we need to use a [[complete]] [[Search Techniques (Search Strategy) (Search Algorithm)]] that will not go into an infinite [[path(s)]]
        > [[Breadth-First Search (BFS)]], [[Iterative-Deepening Search (IDS)]], etc.
        
Don’t really implement [[Inference engines (IE)]]/[[Propositional Logic]] nowadays because everything is already set up for you. [[First-Order Logic]] is more applicable