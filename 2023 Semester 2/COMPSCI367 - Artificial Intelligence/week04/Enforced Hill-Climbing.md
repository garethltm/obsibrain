- You are using [[Hill-Climbing]] algorithm but when stuck instead of terminating, you perform [[Breadth-First Search (BFS)]] from a [[Local Optima]] until you find the next state with better [[heuristic(s)]] function (improvement)
	- good at Escaping Shoulders/[[Local Optima]]![[Pasted image 20231022164039.png]]

Typically,
- prolonged periods of exhaustive search
- bridged by relatively quick periods of [[Hill-Climbing]]
- Sometimes called "Variable Neighbourhood Descent"

>	#Example 
>	![[Untitled.png]]

Middle ground between [[Local Search]] & [[Systematic Search]]
