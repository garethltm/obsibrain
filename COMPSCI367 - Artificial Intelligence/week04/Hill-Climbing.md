- Have no Frontier
- Will just STOP

## Steps
- Start wherever
- Repeat: move to the best neighbouring [[state(s)]]
- If no neighbours better than current → QUIT


*"Like climbing Everest in thick fog with amnesia"*
- algorithm doesn't know what happened before that - NO MEMORY

![[Pasted image 20231022154712.png]]
- IMPORTANCE of [[Hill-Climbing]] = we always want to improve the VALUE

### Difficulties
- Main problem: depending on [[initial state (start state)]], can get stuck in local maxima
![[Pasted image 20231022160343.png]]
> Note: these difficulties apply to all [[Local Search]] algorithms, and usually becomes much worse as the search space becomes higher dimensional

### Problems
1. Local maxima
2. Plateaus
3. [[Diagonal ridges]]

### Summary
- [[Hill-Climbing]] - choose best child
- [[Hill-Climbing with side-way moves]] - choose best or equal child
- [[Enforced Hill-Climbing]] - use [[Breadth-First Search (BFS)]] until you find a "better" node
- [[Tabu Search]] - keeps a [[Tabu list]] of nodes you have been to & don't go back