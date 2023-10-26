A [[Structured Representation]] which represents [[Dependency]] relations among (decision & random variables)
	- reflecting everything in a graph

An extension of a [[Bayesian Networks]] with 3 nodes:
1. [[Decision nodes]]
2. [[Chance nodes]]
3. A single [[utility]] node, represents the [[utility]]
>>	The [[Chance nodes]] take the same tole as nodes in a [[Bayesian Networks]] with [[Local Markov Property]]

>	#Example 
>	![[COMPSCI3672022_S2W12Lecture35Decision2of2-04.jpg]]![[COMPSCI3672022_S2W12Lecture35Decision2of2-06.jpg]]
>	- [[policy]], [[optimal policy]], [[value of a decision network]]
>	- [[SSDN-based one-off decision problem]]

>	#Example 
>	![[COMPSCI3672022_S2W12Lecture35Decision2of2-08.jpg]]![[Pasted image 20231025182314.png]]
>	- basically combining the Acc: 
>	![[Pasted image 20231026163437.png]]
>	into:![[Pasted image 20231026163536.png]]

>	#Example 
>	![[COMPSCI3672022_S2W12Lecture35Decision2of2-15.jpg]]
>	Should an [[agent(s)]] take an umbrella?
>	[[Chance nodes]]: 
>	1. Weather: {*norain, rain*}
>	2. Forecast: {*sunny, cloudy, rainy*}
>	[[Decision nodes]]:
>	Umbrella: {0, 1}
>	![[Pasted image 20231026165531.png]]
>	![[Pasted image 20231026165642.png]]
>	There are 3 types of edges:
>	1. Into a [[Decision nodes]]: available information (observation/memory) when the decision i smake
>	2. Into a [[Chance nodes]]: Probabilistic [[Dependency]]
>	3. Into a [[utility]] node: [[Dependency]] of the [[Utility function]]
>	![[Pasted image 20231026174606.png]]
>	![[COMPSCI3672022_S2W12Lecture35Decision2of2-17.jpg]]
>	
- this one deletes all the [[Chance nodes]]