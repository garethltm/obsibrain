- You are using [[Hill-Climbing]] algorithm when stuck instead of terminating, you perform [[Breadth-First Search (BFS)]] from a [[local optima]] until you find the next state with better h function (improvement)
	- good at Escaping Shoulders/[[Local Optima]]![[Pasted image 20231022164039.png]]

Typically,
- prolonged periods of exhaustive search
- bridged by relatively quick periods of [[Hill-Climbing]]
- Sometimes called "Variable Neighbourhood Descent"

Middle ground between [[Local Search]] & [[Systematic Search]]
