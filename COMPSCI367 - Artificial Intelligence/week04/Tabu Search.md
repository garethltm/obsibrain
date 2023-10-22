- A resolution to the problem of [[Hill-Climbing]] not remembering (because it can end up in the same state)
	- it stores a certain amount of states that we visited then adding the most recent & removing the oldest one
		- which helps to avoid the same states twice
- Prevents returning quickly to the same state
	-  implements a [[Tabu list]]
	- Add most recent state to queue; drop oldest
	- Never make the step that is currently "tabu'ed"

## Properties
- 