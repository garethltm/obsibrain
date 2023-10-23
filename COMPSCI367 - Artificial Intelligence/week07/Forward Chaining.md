Start from [[clause(s)]] in $KB\ \cup\ Percepts$ (related to: [[Inference engines (IE)]] & generate new [[logical consequence]]
Each derivation is built on the [[clause(s)]] in $KB\ \cup\ Percepts$ or the [[clause(s)]] that have already been generated
Use a [[rule of derivation]] for inference

[[Forward Chaining]] applies [[Modus Ponens (MP)]] iteratively to the current [[Knowledge Base (KB)]] to generate a new [[clause(s)]], which are then added to [[Knowledge Base (KB)]]

![[Pasted image 20231024002237.png]]![[Pasted image 20231024002255.png]]

- [[Soundness]] of [[Forward Chaining]]:
	- For any [[Definite clause]] [[Knowledge Base (KB)]], [[Percepts]] & query g
		- $KB\ \cup Percepts\ \vdash g$ ([[Proof procedure]])
		implies that
		- $KB\ \cup Percepts\ \vDash g$ (entails)
		![[Pasted image 20231024002608.png]]

- [[Completeness]] of [[Forward Chaining]]
	- For any [[Knowledge Base (KB)]], [[Percepts]] & query g, 
		- $KB\ \cup Percepts\ \vDash g$ (entails)
		implies
		- $KB\ \cup Percepts\ \vdash g$ ([[Proof procedure]])
		![[Pasted image 20231024002910.png]]
