- The [[ArchiMate Core Framework]] is a framework of 9 cells used to classify elements of the [[ArchiMate]] core language. 
- It is made up of 3 aspects & 3 layers
	![[Pasted image 20240318002539.png]]
- It is important to understand that the classification of elements based on aspects & layers is only a global one. Real-life architecture elements need not strictly be confined to 1 layer or layer because elements that link the different aspects & layers, play a central role in a coherent architectural description

![[Pasted image 20240318002705.png]]

#### The structure of the framework 
- allows for modeling of the enterprise from different viewpoints, where the position within the cells highlights the concerns of the stakeholder. A stakeholder typically can have concerns that cover multiple cells.

#### The dimensions of the framework
1. Layers
	- the 3 levels at which an enterprise can be modeled in [[ArchiMate]] - Business, Application & Technology
2. Aspects
	- [[The Active Structure Aspect]]
	- [[The Behaviour Aspect]]
	- [[The Passive Structure Aspect]]
		the 3 aspects were inspired by natural language where a sentence has:
		1. a subject (active structure)
		2. a verb (behavior)
		3. an object (passive structure)
By using the same constructs that people are used to in their own languages, the [[ArchiMate]] language is easier to learn & read

Since [[ArchiMate]] notation is a graphical language where elements are organized spatially, this order is of no consequence in modeling

![[Pasted image 20240318003711.png]]Alternatively Wierda, puts it this way:
*"Almost all of [[ArchiMate]] is built from 3 types of elements:"*
1. elements that act: active (structure) elements
2. elements that represent the behavior of those 'elements that act': behavioral elements
3. elements that cannot act which are acted upon by that behavior: passive (structural elements)
