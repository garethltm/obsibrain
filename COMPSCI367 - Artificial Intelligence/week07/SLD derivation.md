- [[SLD derivation]] of a query `ask g` from $KB\ \cup\ Percepts$ is a sequence of [[definite clause(s)]] $\gamma0, ...,\gamma n$ :
	- The head of each $\gamma i$ is yes
	- $\gamma 0$ is $yes \leftarrow g$
	- For i >0, $\gamma i$ is obtained by [[resolution]] (at each iteration) from $\gamma i-1$ with a [[definite clause(s)]] in $KB\ \cup\ Percepts$: $$\frac {\gamma i-1,\ a\ clause\ in\ KB\ \cup\ Percepts}{\gamma i}$$![[Pasted image 20231024010025.png]]
>	#Example 
>	![[Pasted image 20231024010105.png]]