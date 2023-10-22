- You are using [[Hill-Climbing]] algorithm when stuck instead of terminating, you perform [[Breadth-First Search (BFS)]] from a local optima until you find the next state with better h function (improvement)
	- good at Escaping Shoulders/[[Local Optima]]

Typically,
- prolonged periods of exhaustive search
- bridged by relatively quick periods of [[Hill-Climbing]]
- Sometimes called "Variable Neighbourhood Descent"

Middle ground 