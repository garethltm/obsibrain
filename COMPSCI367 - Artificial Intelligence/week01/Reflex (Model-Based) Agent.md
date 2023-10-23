- Also known as Model-Based [[agent]]
- most effective way to handle [[Partially Observable]] is for the [[agent]] to keep track of the part of the [[world]] it can't see
- [[agent]] should maintain some sort of internal [[state(s)]]
- Knowledge about "how the [[world]] works" - is called the model of the [[world]]
![[Pasted image 20231012005149.png]]

## Simple Reflex Agent
- they respond directly to [[COMPSCI367 - Artificial Intelligence/week01/Percepts]]

## Limitations
- [[agent]] with a [[world model]] but no planning can look into the past but not the future
- Bad for:
	- Searching several moves ahead
	- Complex [[task(s)]] requiring many individual steps
	- Logical reasoning to achieve goals