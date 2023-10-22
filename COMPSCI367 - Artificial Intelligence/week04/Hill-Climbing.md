- Have no Frontier
- Will just STOP

## Steps
- Start wherever
- Repeat: move to the best neighbouring state
- If no neighbours better than current → QUIT


*"Like climbing Everest in thick fog with amnesia"*
- algorithm doesn't know what happened before that - NO MEMORY

![[Pasted image 20231022154712.png]]
- IMPORTANCE of [[Hill-Climbing]] = we always want to improve the VALUE

### Difficulties
- Main problem: depending on [[initial state]], can get stuck in local maxima
![[Pasted image 20231022160343.png]]
> Note: these difficulties apply to all [[Local Search]] algorithms, and usually becomes much worse as the [[search space]] becomes higher dimensional
1. Local maxima
2. Plateaus
3. [[Diagonal ridges]]