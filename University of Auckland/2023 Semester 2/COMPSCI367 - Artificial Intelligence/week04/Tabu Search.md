- A resolution to the problem of [[Hill-Climbing]] not remembering (because it can end up in the same [[State(s)]] again)
	- it stores a certain amount of [[State(s)]] that we visited then adding the ==most recent & removing the oldest one==
		- which helps to avoid the same [[State(s)]] twice
- Prevents returning quickly to the same [[State(s)]]
	-  implements a [[Tabu list]]
	- Add most recent [[State(s)]] to [[Tabu list]]; drop oldest
	- Never make the step that is currently "tabu'ed"

## Properties
- As the size of the [[Tabu list]] grows, [[Hill-Climbing]] will asymptotically become "non-redundant" (won't look at the same state twice)
- In practice, a reasonable sized [[Tabu list]] (say 100 or so) would improve the performance of [[Hill-Climbing]] in many problems
- The [[Tabu list]] can allow the [[algorithm]] to escape some of the local minima

